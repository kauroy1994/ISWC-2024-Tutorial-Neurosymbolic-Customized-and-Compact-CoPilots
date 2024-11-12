# Neurosymbolic Customized and Compact CoPilots 
ℹ️ Authors: [Kaushik Roy](https://kauroy1994.github.io/home/), [Megha Chakraborty](https://scholar.google.com/citations?hl=en&user=Jqq0mHoAAAAJ), [Yuxin Zi](http://linkedin.com/in/yuxin-zi), [Manas Gaur](https://cs.umbc.edu/manas), and [Amit Sheth](http://aiisc.ai/amit)

📰 Preprint link: [Neurosymbolic Customized and Compact CoPilots](https://scholarcommons.sc.edu/cgi/viewcontent.cgi?article=1628&context=aii_fac_pub)

## Tutorial Details
### Detailed Program
 - Part 1: (20 mins) Neurosymbolic Customized and Compact Copilots
 -  Part 2 (20 Mins) - Use Case Example: Multi Tiered System of Supports (MTSS)
 -  Part 3 (40 Mins) - Demonstrating Preliminary NeSy-CC Copilots (MTSS)
 -  Part 4 (20 Mins) - Future Work and Vision (MTSS)
   
### Tutorial date and time: Nov 12th 2024, 11am-12:40pm
### Slides🔜  [Link](https://docs.google.com/presentation/d/1f_3LwvoARdOw7H_fHLMn20IUdwXbHltDnGTdS6M5jYg/edit?usp=sharing)

## Abstract
Large Language Models (LLMs) are credible with open-domain interactions such as question answering, summarization, and explanation generation [1]. LLM reasoning is based on parametrized knowledge, and as a consequence, the models often produce absurdities and inconsistencies in outputs (eg, hallucinations and confirmation biases)[2]. In essence, they are fundamentally hard to control to prevent off-the-rails behaviors, are hard to fine-tune, customize for tailored needs, prompt effectively (due to the “tug-of-war” between external and parametric memory), and extremely resource-hungry due to the enormous size of their extensive parametric configurations [3, 4]. Thus, significant challenges arise when these models are required to perform in critical applications in domains such as healthcare and finance, that need better guarantees and in turn, need to support grounding, alignment, and instructibility. AI models for such critical applications should be customizable or tailored as appropriate for supporting user assistance in various tasks, compact to perform in real-world resource-constraint settings, and capable of controlled, robust, reliable, interpretable, and grounded reasoning (grounded in rules, guidelines, and protocols)[5]. This special session explores the development of compact, custom neurosymbolic AI models and their use through human-in-the-loop co-pilots for use in critical applications [6].

### References
1. Wayne Xin Zhao, Kun Zhou, Junyi Li, Tianyi Tang, Xiaolei Wang, Yupeng Hou, Yingqian Min, Beichen Zhang, Junjie Zhang, Zican Dong, et al. A survey of large language models. arXiv preprint arXiv:2303.18223, 2023.
2. Vipula Rawte, Amit Sheth, and Amitava Das. A survey of hallucination in large foundation models. arXiv preprint arXiv:2309.05922, 2023.
3. Kevin Wu, Eric Wu, and James Zou. How faithful are rag models? quantifying the tug-of-war between rag and llms’ internal prior. arXiv preprint arXiv:2404.10198, 2024.
4. Zhuoran Jin, Pengfei Cao, Yubo Chen, Kang Liu, Xiaojian Jiang, Jiexin Xu, Qiuxia Li, and Jun Zhao. Tug-of-war between knowledge: Exploring and resolving knowledge conflicts in retrieval-augmented language models. arXiv preprint arXiv:2402.14409, 2024.
5. Amit Sheth, Manas Gaur, Kaushik Roy, Revathy Venkataraman, and Vedant Khandelwal. Process knowledge-infused ai: Toward user-level explainability, interpretability, and safety. IEEE Internet Computing, 2022.
6. Amit Sheth, Kaushik Roy, and Manas Gaur. Neurosymbolic artificial intelligence (why, what, and how). IEEE Intelligent Systems, 38(3):56–62, 2023.

## 🤖 Copilot Examples
#### 🥣 Nourish Co-pilot: Custom, Compact, and NeuroSymbolic Diet AI Model

Can I eat this food or not? Does it have ingredients I'm allergic to? How can I make this more nutritious or vegan or keto-free? Does this recipe conform to diabetes guidelines? These are simple yet powerful questions that we ask about our food. To answer these questions and more, we introduce: 

We introduce 𝙉𝙤𝙪𝙧𝙞𝙘𝙝: 𝘼 𝘾𝙪𝙨𝙩𝙤𝙢, 𝘾𝙤𝙢𝙥𝙖𝙘𝙩 𝙖𝙣𝙙 𝙉𝙚𝙪𝙧𝙤𝙨𝙮𝙢𝙗𝙤𝙡𝙞𝙘 𝘿𝙞𝙚𝙩 𝘼𝙄 𝙢𝙤𝙙𝙚𝙡 - That analyses the suitability of a given recipe by analyzing ingredients and cooking actions in multiple contexts. The system also provides explanations in the form of reasoning to the users. Given a recipe is not suitable, the system aims to provide alternative recipes or ingredient substitutions.

Visit here for the demo: [Demo link](https://lnkd.in/eBJhiBDJ)

🔧 𝘾𝙪𝙨𝙩𝙤𝙢: Tailored to analyze and reason over the suitability of a recipe for diabetes and provide alternative recipes or ingredient and cooking action substitutions.

⚙️ 𝘾𝙤𝙢𝙥𝙖𝙘𝙩: Lightweight and cost-effective model, optimized for real-time deployment on consumer-grade hardware

🧠 𝙉𝙚𝙪𝙧𝙤𝙨𝙮𝙢𝙗𝙤𝙡𝙞𝙘: An explainable food recommendation framework that adapts semantic, perceptual, and cognitive framework to ground data with semantic knowledge (semantics), mapping grounded data to disease context (perceptual) and provides reasoning for the recommendation(cognitive) to the users along with the source of knowledge utilized for recommendations. 

#### ❤️ MTSS Co-pilot: Custom, Compact and Neurosymbolic Behavioral Health Assistance Management

**The Multi-Tiered System of Support (MTSS)** framework is designed to assist students with behavioral strategies by drawing on the support of a network that includes parents, counselors, and school administrators. 
🚀 However, the intricate nature of the MTSS structure can overwhelm the support network when addressing a student's case due to the numerous options available. 
🚀 We introduce MTSS-CoPilot, a digital assistant designed to provide essential decision support to the members of a student's support network. This assistant employs an innovative AI approach that ensures its outputs are tailored to the specific needs of the support network, align with expert knowledge, and remain transparent and explainable.

Visit here for the demo: [Demo link](https://lnkd.in/enrFJUeZ)

🔧 𝘾𝙪𝙨𝙩𝙤𝙢: Tailored to solve specific industry challenges (here focused on student-behavioral health support leveraging various members in the student’s support network), providing focused and practical solutions.

⚙️ 𝘾𝙤𝙢𝙥𝙖𝙘𝙩: Lightweight and cost-effective, optimized for real-time deployment on consumer-grade hardware.

🧠 𝙉𝙚𝙪𝙧𝙤𝙨𝙮𝙢𝙗𝙤𝙡𝙞𝙘: Utilizes advanced reasoning capabilities over carefully curated assets, including specialized data, domain knowledge, and human expertise. This ensures the system delivers reliable and safe outputs by adhering to these curated resources.

### Code🔜 
* [Github](https://github.com/kauroy1994/ISWC-2024-Tutorial-Neurosymbolic-Customized-and-Compact-CoPilots)
* [Versions](https://github.com/kauroy1994/MTSS-Copilots)
* Convert to QA
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
* Judge LLM
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
