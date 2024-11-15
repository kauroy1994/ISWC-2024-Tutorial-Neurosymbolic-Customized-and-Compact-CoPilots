# 💻 Code Snippets and Quick Links
* [Github](https://github.com/kauroy1994/ISWC-2024-Tutorial-Neurosymbolic-Customized-and-Compact-CoPilots)
* [Versions](https://github.com/kauroy1994/MTSS-Copilots)
## **Convert to QA Code Snippet**
  ```python
  from typing import List
  import json
  from pydantic import BaseModel
  from groq import Groq
  
  groq = Groq(api_key=GROQ_API_KEY)
  
  # Define the data model for question and answer pairs
  class QuestionAnswer(BaseModel):
      question: str
      answer: str
  
  class QAResponse(BaseModel):
      qa_pairs: List[QuestionAnswer]

  def get_qa_pairs(text: str) -> QAResponse:
      chat_completion = groq.chat.completions.create(
          messages=[
              {
                  "role": "system",
                  "content": "You are a helpful assistant that generates question-and-answer pairs in JSON format.\n"
                  f"The JSON object must follow this schema: {json.dumps(QAResponse.model_json_schema(), indent=2)}",
              },
              {
                  "role": "user",
                  "content": f"Generate question and answer pairs for the following text:\n\n{text}",
              },
          ],
          model="llama3-8b-8192",
          temperature=0.0,
          stream=False,
          response_format={"type": "json_object"},
      )
      return QAResponse.model_validate_json(chat_completion.choices[0].message.content)

  def print_qa_pairs(qa_response: QAResponse):
      print("Question and Answer Pairs:")
      for pair in qa_response.qa_pairs:
          print(f"Q: {pair.question}")
          print(f"A: {pair.answer}")
          print()

  # Example usage
  text_input = """
  MTSS stands for Multi-Tiered System of Supports, a framework that helps schools and districts support students' needs through research-based strategies. MTSS aims to improve student achievement and social and emotional competencies by: 
   
  Providing equitable access to instruction and support 
   
  Creating nurturing learning environments 
   
  Integrating education, health, and human services systems 
   
  Using data to inform decision-making 
   
  MTSS is based on a public health approach and includes four key components: screening, progress monitoring, multi-level prevention system, and data-based decision making. 
   
  MTSS can also help identify students with learning or other disabilities, depending on state law. MTSS began as Response to Instruction and Intervention (RTI), which was intended to replace the practice of labeling students as having learning disabilities.
  """
  
  qa_response = get_qa_pairs(text_input)
  print_qa_pairs(qa_response)
  ```
## **Judge LLM Code Snippet**
  ```python
  from typing import Optional
  import json
  from pydantic import BaseModel
  from groq import Groq
  
  # Initialize the main and judge LLM clients
  main_llm = Groq()
  judge_llm = Groq()
  
  # Define the data model for judgment
  class JudgeResponse(BaseModel):
      is_accurate: bool
      score: float  # A score between 0 and 1, where 1 is fully accurate
      comment: Optional[str]
  
  def generate_response(prompt: str) -> str:
      # Generate a response using the main LLM
      chat_completion = main_llm.chat.completions.create(
          messages=[
              {
                  "role": "system",
                  "content": "You are a helpful assistant that answers questions.",
              },
              {
                  "role": "user",
                  "content": prompt,
              },
          ],
          model="llama3-8b-8192",
          temperature=0.5,
          stream=False,
      )
      return chat_completion.choices[0].message.content
  
  def judge_response(prompt: str, response: str) -> JudgeResponse:
      # Use the judge LLM to evaluate the accuracy of the response
      chat_completion = judge_llm.chat.completions.create(
          messages=[
              {
                  "role": "system",
                  "content": "You are an expert judge that evaluates the accuracy of responses.\n"
                  f"The JSON object must follow this schema: {json.dumps(JudgeResponse.model_json_schema(), indent=2)}",
              },
              {
                  "role": "user",
                  "content": f"""
                  Given the following prompt and response, evaluate the response for its accuracy.
                  Return your evaluation as JSON, specifying whether the response is accurate (true or false),
                  a score between 0 and 1 where 1 is fully accurate, and an optional comment.
                  
                  Prompt: "{prompt}"
                  Response: "{response}"
                  """,
              },
          ],
          model="llama3-8b-8192",
          temperature=0,
          stream=False,
          response_format={"type": "json_object"},
      )
      return JudgeResponse.model_validate_json(chat_completion.choices[0].message.content)

    def evaluate_llm_response(prompt: str):
        # Generate a response from the main LLM
        response = generate_response(prompt)
        print("Generated Response:")
        print(response)
    
        # Judge the accuracy of the response
        judgment = judge_response(prompt, response)
        print("\nJudgment:")
        print(f"Is Accurate: {judgment.is_accurate}")
        print(f"Score: {judgment.score}")
        if judgment.comment:
            print(f"Comment: {judgment.comment}")
    
    # Example usage
    prompt = "Explain the importance of fast language models."
    evaluate_llm_response(prompt)
  ```
