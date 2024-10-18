# Neurosymbolic Customized and Compact CoPilots 
ℹ️ Authors: [Kaushik Roy](https://kauroy1994.github.io/home/), [Megha Chakraborty](https://scholar.google.com/citations?hl=en&user=Jqq0mHoAAAAJ), [Yuxin Zi](http://linkedin.com/in/yuxin-zi), [Manas Gaur](https://cs.umbc.edu/manas), and [Amit Sheth](http://aiisc.ai/amit)

📰 Preprint link: [Neurosymbolic Customized and Compact CoPilots](https://scholarcommons.sc.edu/cgi/viewcontent.cgi?article=1628&context=aii_fac_pub)



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

## Method and Applications Details

### Key Features for The Proposed Copilots

| **Feature**           | **Feature Description**                                                                                                                                                             | **Example from Copilot Concept**                                                                                                                                                                             | **How?**                                                                                                                                                                                                                                                                                                                                                                    |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Alignment**                       | Ensuring that AI systems are designed and operate consistently with the enterprise's goals, values, and ethics, while also providing metrics for evaluating alignment with objectives. | **MTSS-CoPilot**: The system aligns behavioral health support with specific student needs by tailoring outputs to members of the support network.                                                                                         | The MTSS-CoPilot ensures alignment by focusing on the specific challenges faced in student behavioral health management. It provides recommendations that are consistent with expert knowledge and tailored to the network’s needs, ensuring adherence to the support system's long-term goals while considering short-term challenges.                                             |
| **Grounding**                       | Refers to connecting AI outputs to real-world concepts, data, and actions to ensure relevance and accuracy, which includes training AI on domain-specific data.                        | **Nourich**: Analyses ingredients and cooking actions in the context of specific health guidelines like diabetes.                                                                                             | Nourich grounds its recommendations by incorporating health-specific contexts (like diabetes) into its analysis, mapping the data to real-world dietary needs. This ensures that the AI recommendations are relevant to the user’s health status, thereby improving decision-making around food choices based on grounded, domain-specific data.                                        |
| **Instructability**                 | The ability of an AI system to accept instructions from users and adapt its behavior, often by allowing symbolic input to override statistical models when needed.                     | **SmartPilot**: Allows for domain experts in manufacturing to influence AI outputs by integrating human expertise for handling rare events in assembly processes.                                                   | The SmartPilot system incorporates expert knowledge and provides mechanisms for human operators to adjust AI behavior when encountering rare events in the assembly process. This enables instructability by letting users guide the AI, ensuring decisions remain aligned with operational realities and domain-specific nuances in manufacturing.                                      |
| **Explainability and Interpretability** | The capability of an AI system to provide understandable reasons for its decisions or predictions, ensuring transparency for both technical and non-technical users.                    | **Nourich**: Provides reasoning and explanations behind the suitability of a recipe, including ingredient alternatives and the reasoning behind recommendations.                                               | Nourich focuses on explainability by offering clear justifications for its decisions. For instance, if a recipe does not suit a user’s dietary guidelines, the system provides alternative ingredients and a detailed reasoning process. This aligns with the need for AI systems to be transparent and interpretable, especially in sensitive areas like health and nutrition.                   |
| **Safety**                          | Ensuring AI systems operate without causing unintended harm, including implementing fail-safe mechanisms and rigorous testing before deployment.                                      | **MTSS-CoPilot**: Ensures that interventions are safe and reliable, following expert guidelines when supporting student behavior.                                                                             | MTSS-CoPilot emphasizes safety by adhering to carefully curated expert knowledge, ensuring that the recommendations it provides are safe, effective, and in line with educational and behavioral standards. It includes validation mechanisms to avoid unintended consequences in student support.                                                                                          |
| **Abstraction**                     | The process of simplifying complex real-world data and situations to allow AI systems to focus on relevant features for decision-making.                                               | **SmartPilot**: Handles complex scenarios such as rare manufacturing events by abstracting key data from historical and real-time sources for actionable insights.                                               | SmartPilot utilizes abstraction by synthesizing real-time data and historical information, simplifying complex manufacturing scenarios (e.g., rare events) into actionable insights. This allows the system to focus on the relevant features of a process, offering a streamlined approach to problem-solving in complex environments like manufacturing.                                    |
| **Robustness**                      | The ability of AI systems to operate reliably in diverse, unpredictable, and adverse conditions while maintaining accuracy and stability.                                               | **MTSS-CoPilot**: Built to adapt to various case complexities in behavioral management, ensuring the system can handle diverse, unpredictable student cases.                                                    | The MTSS-CoPilot demonstrates robustness by being able to adapt to diverse and unpredictable student cases within the behavioral health context. Its capacity to handle different levels of intervention based on the unique needs of each student reflects the system's ability to manage uncertainty and maintain reliability in real-world scenarios.                                |
| **Custom, Neurosymbolic, and Compact**| Describes methods focused on creating AI systems that are tailored to specific industry needs, use neurosymbolic reasoning for explainability, and are optimized for lightweight deployment. | **Nourich, MTSS-CoPilot, and SmartPilot**: All systems are built as custom solutions tailored to specific industries, using neurosymbolic reasoning for explainability, and optimized for lightweight deployment. | Each copilot is custom-built to address specific industry needs, using neurosymbolic AI for enhanced reasoning and explanation. The systems are compact, meaning they are lightweight and optimized for real-time use on consumer-grade hardware, aligning with the principles of being cost-effective and accessible for real-world applications.                                          |

### Platform for Effective Research and Development of The Proposed Copilots

| **Platform Component**          | **Copilot Development Role**                                                                                                                                                                                                                   | **Development Life-Cycle**                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Logging Engine**              | **Tracks Explicit and Implicit Interactions**: Tracks user interactions with the copilots (e.g., providing dietary preferences for Nourich or selecting behavioral interventions in MTSS-CoPilot) using APIs. Captures feedback, inputs, and system adjustments. | 1. **Initialization**: REST APIs are set up to capture user actions (e.g., querying the copilot, providing input data). <br> 2. **Tracking**: As users interact with the copilots, explicit (direct inputs) and implicit (usage patterns) data is logged. <br> 3. **Feedback Loop**: Logged data is continuously analyzed for trends to optimize interactions and performance over time. |
| **Metadata Store**              | **Tracks ML Model Performance and Development History**: Stores information on ML models, including metrics, parameters, and versions (e.g., Nourich’s dietary analysis model, MTSS-CoPilot’s behavioral model). Uses tools like MLflow for tracking. | 1. **Model Training**: During training of the models, metadata such as hyperparameters, training data version, and performance metrics (accuracy, precision) are logged in the metadata store. <br> 2. **Version Control**: All model versions are tracked over time. <br> 3. **Optimization**: When new models are developed or tuned, previous versions and their performance are analyzed for improvements. |
| **Query Cache Layer**           | **Enables Fast Retrieval of Information and Knowledge Graphs**: Uses a graph database to cache queries and responses, optimizing performance for recurring or related queries (e.g., retrieving recipe suggestions in Nourich, student profiles in MTSS-CoPilot). | 1. **Data Loading**: Relevant data (e.g., recipe or student profile data) is loaded into the graph database. <br> 2. **Query Execution**: Queries from the copilot are cached for rapid retrieval (e.g., common ingredients or frequent student behavioral cases). <br> 3. **Cache Optimization**: Queries are periodically analyzed to determine if cache performance can be optimized further. |
| **Artifact Store**              | **Stores Artifacts Related to ML Models and Data**: Manages datasets, model artifacts, and outputs using tools like DVC (e.g., training data for Nourich, intervention data for MTSS-CoPilot).                                                     | 1. **Data Versioning**: Data used for training, validation, and testing is version-controlled, allowing developers to track changes over time. <br> 2. **Model Storage**: Trained models and their artifacts are stored, with metadata linking them to specific datasets and experiment parameters. <br> 3. **Artifact Analysis**: Stored artifacts are analyzed to improve model performance, with easy rollback to prior versions if needed. |
| **Source Control**              | **Manages Code and Collaboration**: Source control, such as Git, is used to manage code versions, collaboration, and changes in model architecture or functionality (e.g., behavioral logic in MTSS-CoPilot, nutrition analysis algorithms in Nourich). | 1. **Code Development**: Code for the copilots is developed, committed, and versioned using Git. <br> 2. **Collaboration**: Multiple developers can work on different parts of the copilots, merging changes through pull requests. <br> 3. **Bug Tracking**: Issues and bugs are tracked, with the ability to roll back to earlier stable versions as needed. Continuous integration ensures safe deployment of changes. |
| **Optimization Engine**         | **Optimizes Performance for Real-time Applications**: Manages model and query optimizations (e.g., ensuring Nourich can run real-time recipe analysis efficiently, improving decision response time for MTSS-CoPilot).                            | 1. **Initial Optimization**: The optimization engine analyzes model and system performance metrics (e.g., query response time, memory usage) and adjusts parameters to optimize performance. <br> 2. **Ongoing Tuning**: As new data is added and the system evolves, the optimization engine continues to fine-tune the model's parameters and architecture. <br> 3. **Performance Monitoring**: The engine monitors long-term performance metrics to maintain efficiency. |
| **Query Engine**                | **Executes Queries Against Metadata and Open-source Documents**: Executes queries related to metadata stored in the platform (e.g., query nutritional guidelines for Nourich, behavioral protocols for MTSS-CoPilot).                           | 1. **Query Execution**: Queries against metadata (e.g., querying the MLflow store for model performance) or external knowledge sources (e.g., diabetes guidelines) are executed. <br> 2. **Data Integration**: Results are integrated into the copilots' decision-making process. <br> 3. **Continuous Learning**: As new documents and data become available, the query engine continuously adapts its knowledge base and response capability. |

### Example Development Life-cycle for Nourich

1. **Initial Setup**:
   - Define the overall goal (e.g., to analyze recipes based on specific dietary needs).
   - Set up Git for source control and the logging engine for tracking user interactions (e.g., user inputs preferences for vegan diets).
   - Configure the artifact store for dataset versioning (e.g., initial training dataset with food and nutrition data) and store ML model artifacts.

2. **Model Training**:
   - Use the metadata store (MLflow) to track hyperparameters and performance metrics as the Nourich model is trained on different dietary datasets.
   - Cache frequent queries using the query cache layer (e.g., queries related to common allergies or popular diet plans).

3. **System Optimization**:
   - Deploy the initial version of Nourich, using the optimization engine to tune for real-time response and efficient recipe recommendations.
   - Query open-source documents (e.g., nutritional guidelines) to update and improve the copilot’s reasoning capabilities.

4. **Continuous Improvement**:
   - As users interact with Nourich, the logging engine tracks user inputs (e.g., modifications to dietary preferences) and the system adapts over time.
   - Regular model updates and optimizations are performed, with data artifacts version-controlled and previous model performance stored for reference.
   - Continuous feedback from the query engine and logging platform helps to improve the copilot's recommendations, enhancing overall user satisfaction. 

This process would be similar for other copilots like MTSS-CoPilot and SmartPilot, but with a focus on the specific domain (behavioral health management or manufacturing optimization, respectively).

## 📰 Slides
🔜 Comming soon .. 

## 💻 Preliminary Experiments - Neuro-Symbolic Question-Answer Knowledge Search System [[Code](https://github.com/kauroy1994/MTSS-Copilots/tree/kaushik_code_v2)]

This experiment implements a **Question-Answer Knowledge Search System** using **neuro-symbolic AI** principles. The system processes queries, retrieves relevant questions from a user-provided QA dataset, and generates a knowledge panel with extracted entities and relationships. The architecture effectively combines **neural network-based** language understanding and **symbolic reasoning** for precise query answering.

### Key Features

- **Neuro-Symbolic Design**: Combines the strengths of neural methods (deep learning models for sentence embeddings) with symbolic reasoning (knowledge graph-based similarity).
- **User-Customizable**: The system dynamically adapts to the user's **QA dataset** in JSON format and extracts insights from the provided questions and answers.
- **Compact and Efficient**: Utilizes **lightweight models** such as `MiniLM-L6-v2` with relatively modest parameters, ensuring fast performance and lower computational costs.

### Architecture Overview

#### 1. **Neuro-Symbolic Design**
The system leverages a **neuro-symbolic approach**, which combines:
   - **Neural Networks**: We use **SentenceTransformers** to generate dense embeddings for the questions and queries. This neural model helps compute similarity scores between the query and dataset questions based on the semantic meaning of sentences.
   - **Symbolic Knowledge Representation**: The system uses **Spacy** to extract **subject-verb-object (SVO)** triples from both the query and the top matched answers. These triples represent relationships and entities in a structured, symbolic manner, forming a lightweight **knowledge graph**.

The combination of these two approaches ensures that the system can:
   - Understand the **semantic meaning** of queries and answers (neural).
   - Reason about the **explicit relationships** between entities (symbolic).

#### 2. **Customization to the User's QA Dataset**

The system is designed to be highly flexible and customizable:
   - It accepts any **JSON-formatted dataset** of questions and answers, which is dynamically processed during runtime. The dataset can include any domain-specific questions and answers, making it adaptable to various contexts (e.g., **tax assistance**, **medical support**, etc.).
   - The user can update the dataset with new questions and answers without modifying the codebase. The system automatically adjusts to the new content and generates results accordingly.

#### 3. **Compactness: Lightweight and Efficient Models**

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
