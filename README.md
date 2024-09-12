# Neurosymbolic Customized and Compact CoPilots 
ℹ️ Authors: [Kaushik Roy](https://kauroy1994.github.io/home/), [Megha Chakraborty](https://scholar.google.com/citations?hl=en&user=Jqq0mHoAAAAJ), [Yuxin Zi](http://linkedin.com/in/yuxin-zi), [Manas Gaur](https://cs.umbc.edu/manas), and [Amit Sheth](http://aiisc.ai/amit)

📰 Preprint link: [Neurosymbolic Customized and Compact CoPilots](https://scholarcommons.sc.edu/cgi/viewcontent.cgi?article=1628&context=aii_fac_pub)



## Tutorial Abstract
Large Language Models (LLMs) are credible with open-domain interactions such as question answering, summarization, and explanation generation [1]. LLM reasoning is based on parametrized knowledge, and as a consequence, the models often produce absurdities and inconsistencies in outputs (eg, hallucinations and confirmation biases)[2]. In essence, they are fundamentally hard to control to prevent off-the-rails behaviors, are hard to fine-tune, customize for tailored needs, prompt effectively (due to the “tug-of-war” between external and parametric memory), and extremely resource-hungry due to the enormous size of their extensive parametric configurations [3, 4]. Thus, significant challenges arise when these models are required to perform in critical applications in domains such as healthcare and finance, that need better guarantees and in turn, need to support grounding, alignment, and instructibility. AI models for such critical applications should be customizable or tailored as appropriate for supporting user assistance in various tasks, compact to perform in real-world resource-constraint settings, and capable of controlled, robust, reliable, interpretable, and grounded reasoning (grounded in rules, guidelines, and protocols)[5]. This special session explores the development of compact, custom neurosymbolic AI models and their use through human-in-the-loop co-pilots for use in critical applications [6].

### References
1. Wayne Xin Zhao, Kun Zhou, Junyi Li, Tianyi Tang, Xiaolei Wang, Yupeng Hou, Yingqian Min, Beichen Zhang, Junjie Zhang, Zican Dong, et al. A survey of large language models. arXiv preprint arXiv:2303.18223, 2023.
2. Vipula Rawte, Amit Sheth, and Amitava Das. A survey of hallucination in large foundation models. arXiv preprint arXiv:2309.05922, 2023.
3. Kevin Wu, Eric Wu, and James Zou. How faithful are rag models? quantifying the tug-of-war between rag and llms’ internal prior. arXiv preprint arXiv:2404.10198, 2024.
4. Zhuoran Jin, Pengfei Cao, Yubo Chen, Kang Liu, Xiaojian Jiang, Jiexin Xu, Qiuxia Li, and Jun Zhao. Tug-of-war between knowledge: Exploring and resolving knowledge conflicts in retrieval-augmented language models. arXiv preprint arXiv:2402.14409, 2024.
5. Amit Sheth, Manas Gaur, Kaushik Roy, Revathy Venkataraman, and Vedant Khandelwal. Process knowledge-infused ai: Toward user-level explainability, interpretability, and safety. IEEE Internet Computing, 2022.
6. Amit Sheth, Kaushik Roy, and Manas Gaur. Neurosymbolic artificial intelligence (why, what, and how). IEEE Intelligent Systems, 38(3):56–62, 2023.

# Example Scenario
💡 A Vision for a neurosymbolic compact and customized multi-agent copilot framework for facilitating discussions between healthcare professionals by navigating intricate information layers at school and district administration levels in a healthcare system (This example is from the [MTSS system](https://ed.sc.gov/instruction/early-learning-and-literacy/multi-tiered-system-of-supports-mtss/)).

![image](https://github.com/kauroy1994/ISWC-2024-Tutorial-Neurosymbolic-Customized-and-Compact-CoPilots/assets/57400980/be16fb07-30a8-4035-8480-fd0ff1e14064)


## 📰 Slides
🔜 Comming soon .. 

# Neuro-Symbolic Question-Answer Knowledge Search System

This repository implements a **Question-Answer Knowledge Search System** using **neuro-symbolic AI** principles. The system processes queries, retrieves relevant questions from a user-provided QA dataset, and generates a knowledge panel with extracted entities and relationships. The architecture effectively combines **neural network-based** language understanding and **symbolic reasoning** for precise query answering.

## Key Features

- **Neuro-Symbolic Design**: Combines the strengths of neural methods (deep learning models for sentence embeddings) with symbolic reasoning (knowledge graph-based similarity).
- **User-Customizable**: The system dynamically adapts to the user's **QA dataset** in JSON format and extracts insights from the provided questions and answers.
- **Compact and Efficient**: Utilizes **lightweight models** such as `MiniLM-L6-v2` with relatively modest parameters, ensuring fast performance and lower computational costs.

## Architecture Overview

### 1. **Neuro-Symbolic Design**
The system leverages a **neuro-symbolic approach**, which combines:
   - **Neural Networks**: We use **SentenceTransformers** to generate dense embeddings for the questions and queries. This neural model helps compute similarity scores between the query and dataset questions based on the semantic meaning of sentences.
   - **Symbolic Knowledge Representation**: The system uses **Spacy** to extract **subject-verb-object (SVO)** triples from both the query and the top matched answers. These triples represent relationships and entities in a structured, symbolic manner, forming a lightweight **knowledge graph**.

The combination of these two approaches ensures that the system can:
   - Understand the **semantic meaning** of queries and answers (neural).
   - Reason about the **explicit relationships** between entities (symbolic).

### 2. **Customization to the User's QA Dataset**

The system is designed to be highly flexible and customizable:
   - It accepts any **JSON-formatted dataset** of questions and answers, which is dynamically processed during runtime. The dataset can include any domain-specific questions and answers, making it adaptable to various contexts (e.g., **tax assistance**, **medical support**, etc.).
   - The user can update the dataset with new questions and answers without modifying the codebase. The system automatically adjusts to the new content and generates results accordingly.

### 3. **Compactness: Lightweight and Efficient Models**

Despite its powerful neuro-symbolic design, the system is highly efficient:
   - The **SentenceTransformer model** used in this system, `MiniLM-L6-v2`, is a compact and efficient transformer-based language model with only **33 million parameters**, significantly smaller than many other transformer models like BERT or GPT.
   - The symbolic reasoning component using **Spacy** operates efficiently, extracting relationships from text with minimal computational overhead.

### Design Components

#### Neural Component
- **SentenceTransformers** (`MiniLM-L6-v2`): This model is a **smaller variant** of transformer-based language models. It is optimized for efficiency and speed, making it a great choice for systems where performance and low resource consumption are important.
- The model generates **semantic embeddings** for both the user's query and the dataset questions. These embeddings allow the system to measure **semantic similarity** using **cosine similarity**.

#### Symbolic Component
- **Spacy**: We use Spacy to extract **SVO (subject-verb-object) triples** from the query and the matched answers. These triples are then compared to calculate a **knowledge-graph-based similarity** between the query and answers.
- This **symbolic reasoning** enhances the system's interpretability and allows it to handle **structural relationships** in the text.

### Query Filtering Mechanism

To ensure the system only provides relevant answers, a filtering mechanism is applied:
- **Neural Similarity**: Queries must pass a neural similarity threshold. If the neural similarity score between the query and the dataset questions is below a certain threshold (e.g., **0.6**), the system responds with a boilerplate message.
- **Knowledge Graph Similarity**: If the query passes the neural threshold, the system checks the similarity between **SVO triples** extracted from the query and the matched answer. If this knowledge-graph similarity score is below a threshold (e.g., **0.5**), the system returns a boilerplate response: *"Sorry, we don't have sufficient information to answer this query."*

This dual filtering ensures that only **relevant and accurate answers** are provided to the user.

### Usage

#### Setup and Customization

1. **Customize the Dataset**: 
   - To use the system, simply provide a **JSON file** containing your domain-specific **questions and answers**. The system will adapt to any content you provide without requiring code changes.

   Example JSON format:
   ```json
   [
       {
           "question": "What is the role of administrators in MTSS?",
           "answer": "Administrators oversee the MTSS process and ensure resources are allocated."
       },
       {
           "question": "How does MTSS help students?",
           "answer": "MTSS provides targeted interventions based on student performance data."
       }
   ]
   ```

2. **Run the Application**:
   After setting up the dataset and installing dependencies, you can run the Gradio app to interact with the system in a browser.

   ```bash
   python main.py
   ```

#### Query Example:
- **Query**: "How do administrators support the MTSS process?"
- **Top Matched Question**: "What is the role of administrators in MTSS?"
- **Answer**: "Administrators oversee the MTSS process and ensure resources are allocated."
- **Knowledge Panel**: 
  
  **Administrators** oversee **MTSS process**
  

### Requirements

- Python 3.7+
- `gradio`, `spacy`, `sentence-transformers`, `torch`, `matplotlib`, `pillow`, `numpy`

### Efficiency Considerations

- The model uses the **MiniLM-L6-v2**, a transformer model with only **33 million parameters**. This ensures a balance between **performance** and **accuracy** while keeping resource consumption low.
- **Spacy** for symbolic triple extraction is lightweight, ensuring that the symbolic reasoning layer adds minimal overhead.

### Key Features for The Proposed Copilots
Here's a table that aligns examples from the copilot concepts you provided with the sections of the draft article. Each concept is mapped to attributes such as Grounding, Instructability, Alignment, Explainability, and others discussed in the article. 

| **Feature Description**           | **Example from Copilot Concept**                                                                                                                                                                             | **Explanation**                                                                                                                                                                                                                                                                                                                                                                    |
|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Alignment**                       | **MTSS-CoPilot**: The system aligns behavioral health support with specific student needs by tailoring outputs to members of the support network.                                                                                         | The MTSS-CoPilot ensures alignment by focusing on the specific challenges faced in student behavioral health management. It provides recommendations that are consistent with expert knowledge and tailored to the network’s needs, ensuring adherence to the support system's long-term goals while considering short-term challenges.                                             |
| **Grounding**                       | **Nourich**: Analyses ingredients and cooking actions in the context of specific health guidelines like diabetes.                                                                                             | Nourich grounds its recommendations by incorporating health-specific contexts (like diabetes) into its analysis, mapping the data to real-world dietary needs. This ensures that the AI recommendations are relevant to the user’s health status, thereby improving decision-making around food choices based on grounded, domain-specific data.                                        |
| **Instructability**                 | **SmartPilot**: Allows for domain experts in manufacturing to influence AI outputs by integrating human expertise for handling rare events in assembly processes.                                                   | The SmartPilot system incorporates expert knowledge and provides mechanisms for human operators to adjust AI behavior when encountering rare events in the assembly process. This enables instructability by letting users guide the AI, ensuring decisions remain aligned with operational realities and domain-specific nuances in manufacturing.                                      |
| **Explainability and Interpretability** | **Nourich**: Provides reasoning and explanations behind the suitability of a recipe, including ingredient alternatives and the reasoning behind recommendations.                                               | Nourich focuses on explainability by offering clear justifications for its decisions. For instance, if a recipe does not suit a user’s dietary guidelines, the system provides alternative ingredients and a detailed reasoning process. This aligns with the need for AI systems to be transparent and interpretable, especially in sensitive areas like health and nutrition.                   |
| **Safety**                          | **MTSS-CoPilot**: Ensures that interventions are safe and reliable, following expert guidelines when supporting student behavior.                                                                             | MTSS-CoPilot emphasizes safety by adhering to carefully curated expert knowledge, ensuring that the recommendations it provides are safe, effective, and in line with educational and behavioral standards. It includes validation mechanisms to avoid unintended consequences in student support.                                                                                          |
| **Abstraction**                     | **SmartPilot**: Handles complex scenarios such as rare manufacturing events by abstracting key data from historical and real-time sources for actionable insights.                                               | SmartPilot utilizes abstraction by synthesizing real-time data and historical information, simplifying complex manufacturing scenarios (e.g., rare events) into actionable insights. This allows the system to focus on the relevant features of a process, offering a streamlined approach to problem-solving in complex environments like manufacturing.                                    |
| **Robustness**                      | **MTSS-CoPilot**: Built to adapt to various case complexities in behavioral management, ensuring the system can handle diverse, unpredictable student cases.                                                    | The MTSS-CoPilot demonstrates robustness by being able to adapt to diverse and unpredictable student cases within the behavioral health context. Its capacity to handle different levels of intervention based on the unique needs of each student reflects the system's ability to manage uncertainty and maintain reliability in real-world scenarios.                                |
| **Custom, Neurosymbolic, and Compact**| **Nourich, MTSS-CoPilot, and SmartPilot**: All systems are built as custom solutions tailored to specific industries, using neurosymbolic reasoning for explainability, and optimized for lightweight deployment. | Each copilot is custom-built to address specific industry needs, using neurosymbolic AI for enhanced reasoning and explanation. The systems are compact, meaning they are lightweight and optimized for real-time use on consumer-grade hardware, aligning with the principles of being cost-effective and accessible for real-world applications.                                          |
