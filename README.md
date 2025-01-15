# Agentic Retrieval-Augmented Generation (RAG): A Comprehensive Survey

This repository accompanies the paper "Agentic Retrieval-Augmented Generation (RAG): A Comprehensive Survey," providing supplementary materials, visualizations, and insights into the taxonomy, applications, and challenges of Agentic RAG systems. The goal is to facilitate understanding and adoption of these advanced paradigms by researchers and practitioners.

---

## Abstract

Agentic Retrieval-Augmented Generation (RAG) represents a transformative leap in artificial intelligence by embedding autonomous agents into the RAG pipeline. This repository complements the survey paper "Agentic Retrieval-Augmented Generation (RAG): A Comprehensive Survey," providing insights into:

- Foundational principles, including **Agentic Patterns** such as reflection, planning, tool use, and multi-agent collaboration.
- A detailed taxonomy of Agentic RAG systems, showcasing frameworks like single-agent, multi-agent, hierarchical, corrective, adaptive, and graph-based RAG.
- Comparative analysis of traditional RAG, Agentic RAG, and Agentic Document Workflows (ADW) to highlight their strengths, weaknesses, and best-fit scenarios.
- Real-world applications across industries like healthcare, education, finance, and legal analysis.
- Challenges and future directions in scaling, ethical AI, multimodal integration, and human-agent collaboration.

This repository serves as a comprehensive resource for researchers and practitioners to explore, implement, and advance the capabilities of Agentic RAG systems.

---

## Table of Contents
1. 📜 [Abstract](#abstract)
2. 🧩 [Introduction](#introduction)
3. 🤖 [Agentic Patterns](#agentic-patterns-in-retrieval-augmented-generation)
4. 🛠️ [Taxonomy of Agentic RAG Systems](#taxonomy-of-agentic-rag-systems)
5. 🔍 [Comparative Analysis of Agentic RAG Frameworks](#comparative-analysis-of-agentic-rag-frameworks)
6. 💼 [Applications](#applications)
7. 🚧 [Challenges and Future Directions](#challenges-and-future-directions)
8. 📚 [References](#references)
9. 🖊️ [How to Cite](#how-to-cite)
10. 📞 [Contact Information](#contact-information)
11. 📜 [License](#license)

---

## Introduction

Retrieval-Augmented Generation (RAG) systems combine the capabilities of large language models (LLMs) with retrieval mechanisms to generate contextually relevant and accurate responses. While traditional RAG systems excel in knowledge retrieval and generation, they often fall short in handling dynamic, multi-step reasoning tasks, adaptability, and orchestration for complex workflows.

**Agentic Retrieval-Augmented Generation (Agentic RAG)** overcomes these limitations by integrating autonomous AI agents. These agents employ core **Agentic Patterns**, such as reflection, planning, tool use, and multi-agent collaboration, to dynamically adapt to task-specific requirements and provide superior performance in:

- Multi-domain knowledge retrieval.
- Real-time, document-centric workflows.
- Scalable, adaptive, and ethical AI systems.

This repository explores the evolution of RAG to Agentic RAG, presenting:
- **Agentic Patterns**: The core principles driving the system’s adaptability and intelligence.
- **Taxonomy**: A comprehensive classification of Agentic RAG architectures.
- **Comparative Analysis**: Key differences between Traditional RAG, Agentic RAG, and ADW.
- **Applications**: Practical use cases across healthcare, education, finance, and more.
- **Challenges and Future Directions**: Addressing scalability, ethical AI, and multimodal integration.

Whether you’re a researcher, developer, or practitioner, this repository offers valuable insights and resources to understand and advance Agentic RAG systems.

---

## Agentic Patterns in Retrieval-Augmented Generation

Agentic RAG systems derive their intelligence and adaptability from well-defined agentic patterns. These patterns enable agents to handle complex reasoning tasks, adapt to dynamic environments, and collaborate effectively. Below are the key patterns central to Agentic RAG:

### 1. Reflection
- **Definition**: Agents evaluate their own decisions and outputs, identifying errors and areas for improvement.
- **Key Benefits**:
  - Enables iterative refinement of results.
  - Enhances accuracy in multi-step reasoning tasks.
- **Example**: In a medical diagnostic system, agents refine diagnoses based on iterative feedback from retrieved data.

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block;">
  <img src="./assets/agentic_self_reflection.png" alt="Reflection Pattern" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 1: Reflection Pattern</em></p>
</div>

<br><br>

### 2. Planning
- **Definition**: Agents create structured workflows and task sequences to solve problems efficiently.
- **Key Benefits**:
  - Facilitates multi-step reasoning by breaking down tasks.
  - Reduces computational overhead through optimized task prioritization.
- **Example**: A financial analysis system plans data retrieval tasks to assess risks and provide recommendations.

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block;">
  <img src="./assets/agentic_planning.png" alt="Planning Pattern" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 2: Planning Pattern</em></p>
</div>

<br><br>

### 3. Tool Use
- **Definition**: Agents interact with external tools, APIs, and knowledge bases to retrieve and process data.
- **Key Benefits**:
  - Expands the system's capabilities beyond pre-trained knowledge.
  - Enables domain-specific applications by integrating external resources.
- **Example**: A legal assistant agent retrieves clauses from contract databases and applies domain-specific rules for compliance analysis.

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block;">
  <img src="./assets/agentic_tool_use.png" alt="Tool Use Pattern" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 3: Tool Use Pattern</em></p>
</div>

<br><br>

### 4. Multi-Agent Collaboration
- **Definition**: Multiple agents collaborate to divide and conquer complex tasks, sharing information and results.
- **Key Benefits**:
  - Handles large-scale and distributed problems efficiently.
  - Combines specialized agent capabilities for better outcomes.
- **Example**: In customer support, agents collaborate to retrieve knowledge from FAQs, generate responses, and provide follow-ups.

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block;">
  <img src="./assets/multi_agent_pattern.png" alt="Multi-Agent Collaboration Pattern" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 4: Multi-Agent Collaboration Pattern</em></p>
</div>

---

### Significance of Agentic Patterns
These patterns form the backbone of Agentic RAG systems, enabling them to:
- Adapt dynamically to task requirements.
- Improve decision-making through self-evaluation.
- Leverage external resources for domain-specific reasoning.
- Handle complex, distributed workflows via collaboration.

---

## Taxonomy of Agentic RAG Systems

Agentic Retrieval-Augmented Generation (RAG) systems encompass various architectures and workflows, each tailored to specific tasks and levels of complexity. Below is a detailed taxonomy of these systems:

### 1. Single-Agent RAG
- **Key Idea**: A single autonomous agent manages the retrieval and generation process.
- **Workflow**:
  1. Query is submitted to the agent.
  2. The agent retrieves relevant data from external sources.
  3. Data is processed and synthesized into a response.
- **Advantages**:
  - Simple architecture for basic use cases.
  - Easy to implement and maintain.
- **Limitations**:
  - Limited scalability.
  - Ineffective for multi-step reasoning or large datasets.

### 2. Multi-Agent RAG
- **Key Idea**: A team of agents collaborates to perform complex retrieval and reasoning tasks.
- **Workflow**:
  1. Agents dynamically divide tasks (e.g., retrieval, reasoning, synthesis).
  2. Each agent specializes in a specific sub-task.
  3. Results are aggregated and synthesized into a coherent output.
- **Advantages**:
  - Better performance for distributed, multi-step tasks.
  - Increased modularity and scalability.
- **Limitations**:
  - Coordination complexity increases with the number of agents.
  - Risk of redundancy or conflicts between agents.

### 3. Hierarchical Agentic RAG
- **Key Idea**: Organizes agents in a hierarchy for better task prioritization and delegation.
- **Workflow**:
  1. A top-level agent orchestrates subtasks among lower-level agents.
  2. Each lower-level agent handles a specific part of the process.
  3. Results are iteratively refined and integrated at higher levels.
- **Advantages**:
  - Scalable for large and complex tasks.
  - Modular design facilitates specialization.
- **Limitations**:
  - Requires sophisticated orchestration mechanisms.
  - Potential bottlenecks at higher levels of the hierarchy.

### 4. Corrective Agentic RAG
- **Key Idea**: Feedback loops enable agents to evaluate and refine their outputs iteratively.
- **Workflow**:
  1. Initial response is generated by the agent.
  2. A critic module evaluates the response for errors or inconsistencies.
  3. The agent refines the response based on feedback.
  4. Steps 2-3 repeat until the output meets quality standards.
- **Advantages**:
  - High accuracy and reliability through iterative improvements.
  - Useful for error-prone or high-stakes tasks.
- **Limitations**:
  - Increased computational overhead.
  - Feedback mechanisms must be well-designed to avoid infinite loops.

### 5. Adaptive Agentic RAG
- **Key Idea**: Dynamically adjusts retrieval strategies and workflows based on task requirements.
- **Workflow**:
  1. The agent assesses the query and its context.
  2. Adapts retrieval strategies in real-time based on available data and user needs.
  3. Synthesizes a response using dynamic workflows.
- **Advantages**:
  - High flexibility for varied tasks and dynamic environments.
  - Improves context relevance and user satisfaction.
- **Limitations**:
  - Challenging to design robust adaptation mechanisms.
  - Computational overhead for real-time adjustments.

### 6. Graph-Based Agentic RAG
Graph-based RAG systems extend traditional RAG by integrating graph-based data structures for advanced reasoning.

#### 6.1 Agent-G: Agentic Framework for Graph RAG
- **Key Idea**: Dynamically assigns tasks to specialized agents using graph knowledge bases and feedback loops.
- **Workflow**:
  1. Extract relationships from graph knowledge bases (e.g., disease-to-symptom mappings).
  2. Complement with unstructured data from external sources.
  3. Use a critic module to validate results and iteratively improve.
- **Advantages**:
  - Combines structured and unstructured data.
  - Modular and scalable for complex tasks.
  - Ensures high accuracy through iterative refinement.

#### 6.2 GeAR: Graph-Enhanced Agent for RAG
- **Key Idea**: Enhances RAG systems with graph expansion techniques and agent-based architectures.
- **Workflow**:
  1. Expand query-related graphs for better relational understanding.
  2. Leverage specialized agents for multi-hop reasoning.
  3. Synthesize graph-structured and unstructured information into responses.
- **Advantages**:
  - Excels in multi-hop reasoning scenarios.
  - Improves accuracy for deep contextual tasks.
  - Dynamically adapts to complex query environments.

### 7. Agentic Document Workflows (ADW)

Agentic Document Workflows (ADW) extend traditional RAG systems by automating document-centric processes with intelligent agents.

#### Workflow
1. **Document Parsing and Structuring**:
   - Extracts structured data from documents like invoices or contracts.
2. **State Maintenance**:
   - Tracks context across multi-step workflows for consistency.
3. **Knowledge Retrieval**:
   - Retrieves relevant references from external sources or domain-specific databases.
4. **Agentic Orchestration**:
   - Applies business rules, performs multi-hop reasoning, and orchestrates external APIs.
5. **Actionable Output Generation**:
   - Produces structured outputs tailored to specific use cases (e.g., reports or summaries).

#### Key Features and Advantages
- **State Maintenance**: Ensures consistency in multi-step workflows.
- **Domain-Specific Intelligence**: Adapts to specialized domains with tailored rules.
- **Scalability**: Handles large-scale document processing efficiently.
- **Enhanced Productivity**: Reduces manual effort and augments human expertise.

---

### Visual Representations

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block; margin: 10px;">
  <img src="./assets/single_agentic_RAG.png" alt="Single-Agent RAG Diagram" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 5: Single-Agent RAG Diagram</em></p>
</div>

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block; margin: 10px;">
  <img src="./assets/multiagent_agentic_rag.png" alt="Multi-Agent RAG Diagram" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 6: Multi-Agent RAG Diagram</em></p>
</div>

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block; margin: 10px;">
  <img src="./assets/hierarchical_agentic_rag.png" alt="Hierarchical RAG Workflow" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 7: Hierarchical RAG Workflow</em></p>
</div>

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block; margin: 10px;">
  <img src="./assets/agent_g.png" alt="Graph-Based RAG Workflow" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 8: Graph-Based RAG Workflow</em></p>
</div>

<div style="border: 1px solid #ddd; padding: 10px; background-color: white; display: inline-block; margin: 10px;">
  <img src="./assets/agentic_doc_workflow.png" alt="ADW Workflow Diagram" style="max-width:100%; height:auto;">
  <p align="center"><em>Figure 9: ADW Workflow Diagram</em></p>
</div>

---

## Comparative Analysis of Agentic RAG Frameworks

The table below provides a comprehensive comparative analysis of the three architectural frameworks: Traditional RAG, Agentic RAG, and Agentic Document Workflows (ADW). This analysis highlights their respective strengths, weaknesses, and best-fit scenarios, offering valuable insights into their applicability across diverse use cases.

| **Feature**                | **Traditional RAG**               | **Agentic RAG**                        | **Agentic Document Workflows (ADW)**  |
|----------------------------|-----------------------------------|----------------------------------------|----------------------------------------|
| **Focus**                  | Isolated retrieval and generation tasks | Multi-agent collaboration and reasoning | Document-centric end-to-end workflows |
| **Context Maintenance**    | Limited                          | Enabled through memory modules         | Maintains state across multi-step workflows |
| **Dynamic Adaptability**   | Minimal                          | High                                   | Tailored to document workflows         |
| **Workflow Orchestration** | Absent                           | Orchestrates multi-agent tasks         | Integrates multi-step document processing |
| **Use of External Tools/APIs** | Basic integration (e.g., retrieval tools) | Extends via tools like APIs and knowledge bases | Deeply integrates business rules and domain-specific tools |
| **Scalability**            | Limited to small datasets or queries | Scalable for multi-agent systems       | Scales for multi-domain enterprise workflows |
| **Complex Reasoning**      | Basic (e.g., simple Q&A)          | Multi-step reasoning with agents       | Structured reasoning across documents  |
| **Primary Applications**   | QA systems, knowledge retrieval   | Multi-domain knowledge and reasoning   | Contract review, invoice processing, claims analysis |
| **Strengths**              | Simplicity, quick setup           | High accuracy, collaborative reasoning | End-to-end automation, domain-specific intelligence |
| **Challenges**             | Poor contextual understanding     | Coordination complexity                | Resource overhead, domain standardization |

---

### Key Takeaways
- **Traditional RAG** is best suited for simpler tasks requiring basic retrieval and generation capabilities.
- **Agentic RAG** excels in multi-agent collaborative reasoning, making it suitable for more complex, multi-domain tasks.
- **Agentic Document Workflows (ADW)** provide tailored, document-centric solutions for enterprise-scale applications like contract analysis and invoice processing.

---

## Applications

Agentic Retrieval-Augmented Generation (RAG) systems have transformative potential across diverse industries, enabling intelligent retrieval, multi-step reasoning, and dynamic adaptation to complex tasks. Below are some key domains where Agentic RAG systems make a significant impact:

### 1. Healthcare and Personalized Medicine
- **Problem**: Rapid retrieval and synthesis of medical knowledge for diagnostics, treatment planning, and research.
- **Applications**:
  - Clinical decision support systems leveraging multi-modal data (e.g., patient records, medical literature).
  - Automating medical report generation with relevant contextual references.
  - Multi-hop reasoning for analyzing complex relationships (e.g., disease-to-symptom mappings or treatment-to-outcome correlations).

### 2. Education and Personalized Learning
- **Problem**: Delivering personalized and adaptive learning experiences for diverse learners.
- **Applications**:
  - Designing intelligent tutors capable of real-time knowledge retrieval and personalized feedback.
  - Generating customized educational content based on student progress and preferences.
  - Multi-agent systems for collaborative learning simulations.

### 3. Legal and Contract Analysis
- **Problem**: Analyzing complex legal documents and extracting actionable insights.
- **Applications**:
  - Contract summarization and clause comparison with contextual alignment to legal standards.
  - Retrieval of precedent cases and regulatory guidelines for compliance.
  - Iterative workflows for identifying inconsistencies or conflicts in contracts.

### 4. Finance and Risk Analysis
- **Problem**: Analyzing large-scale financial datasets and identifying trends, risks, and opportunities.
- **Applications**:
  - Automating the generation of financial summaries and investment recommendations.
  - Real-time fraud detection through multi-step reasoning and data correlation.
  - Scenario-based modeling for risk analysis using graph-based workflows.

### 5. Customer Support and Virtual Assistants
- **Problem**: Providing contextually relevant and dynamic responses to customer queries.
- **Applications**:
  - Building AI-powered virtual assistants for real-time customer support.
  - Adaptive systems that improve responses by learning from user feedback.
  - Multi-agent orchestration for handling complex, multi-query interactions.

### 6. Graph-Enhanced Applications in Multimodal Workflows
- **Problem**: Tackling tasks requiring relational understanding and multi-modal data integration.
- **Applications**:
  - Graph-based retrieval systems for connecting structured and unstructured data.
  - Enhanced reasoning workflows in domains like scientific research and knowledge management.
  - Synthesis of insights across text, images, and structured data for actionable outputs.

### 7. Document-Centric Workflows
- **Problem**: Automating complex workflows involving document parsing, data extraction, and multi-step reasoning.
- **Applications**:
  - **Invoice Payments Workflow**:
    - Parses invoices to extract key details (e.g., invoice number, vendor info, payment terms).
    - Retrieves related vendor contracts to verify terms and compliance.
    - Generates a payment recommendation report, including cost-saving suggestions (e.g., early payment discounts).
  - **Contract Review**:
    - Analyzes legal contracts for critical clauses and compliance issues.
    - Automatically identifies risks and provides actionable recommendations.
  - **Insurance Claims Analysis**:
    - Automates claims review, extracting policy terms and calculating payouts based on predefined rules.
- **Key Advantages**:
  - **State Maintenance**: Tracks the document’s context across workflow stages.
  - **Domain-Specific Intelligence**: Applies tailored rules for industry-specific needs.
  - **Scalability**: Handles large volumes of enterprise documents efficiently.
  - **Enhanced Productivity**: Reduces manual effort and augments human expertise.

---

## Challenges and Future Directions

While Agentic Retrieval-Augmented Generation (RAG) systems show immense promise, there are several challenges and research opportunities that remain unaddressed:

### Challenges
1. **Coordination Complexity in Multi-Agent Systems**:
   - Managing communication and collaboration among multiple agents can lead to inefficiencies and increased computational overhead.
   - Balancing task assignments and resolving conflicts between agents remains a critical issue.

2. **Ethical and Responsible AI**:
   - Ensuring unbiased retrieval and decision-making in sensitive domains like healthcare and finance.
   - Addressing data privacy concerns and building transparent systems that adhere to ethical standards.

3. **Scalability and Latency**:
   - Scaling Agentic RAG systems to handle large datasets and high-volume queries without compromising response times.
   - Addressing latency in multi-agent and graph-based workflows.

4. **Hybrid Human-Agent Collaboration**:
   - Designing systems that effectively integrate human oversight with autonomous agents for tasks requiring domain expertise.
   - Maintaining user trust and control while leveraging the strengths of AI agents.

5. **Expanding Multimodal Capabilities**:
   - Integrating text, image, audio, and video data for richer and more comprehensive outputs.
   - Handling the complexity of multimodal reasoning in real-time applications.

6. **Developing Specialized Benchmarks**:
   - The lack of standardized benchmarks for evaluating Agentic RAG systems across different domains.
   - Designing benchmarks that account for multi-hop reasoning, contextual understanding, and ethical considerations.

---

### Future Directions
1. **Enhanced Agentic Orchestration**:
   - Development of more robust coordination frameworks for hierarchical and multi-agent systems.
   - Incorporating adaptive learning mechanisms to dynamically improve task allocation.

2. **Domain-Specific Applications**:
   - Customizing Agentic RAG systems for niche domains like legal analysis, personalized education, and advanced scientific research.

3. **Ethical AI and Governance Frameworks**:
   - Building tools to monitor, explain, and mitigate biases in AI outputs.
   - Developing policies and guidelines for ethical deployment in high-stakes environments.

4. **Efficient Graph-Based Reasoning**:
   - Optimizing graph-based workflows for large-scale, real-world applications.
   - Exploring hybrid approaches that combine graph-based reasoning with neural networks.

5. **Human-AI Synergy**:
   - Designing intuitive interfaces and workflows to empower humans to interact effectively with Agentic RAG systems.
   - Focusing on explainability and user-centric design.

---

## References

[1] Aditi Singh. Exploring language models: A comprehensive survey and analysis. In 2023 International Conference on Research Methodologies in Knowledge Management, Artificial Intelligence and Telecommunication Engineering (RMKMATE), pages 1–4, 2023.

[2] Wayne Xin Zhao, Kun Zhou, Junyi Li, Tianyi Tang, Xiaolei Wang, Yupeng Hou, Yingqian Min, Beichen Zhang, Junjie Zhang, Zican Dong, Yifan Du, Chen Yang, Yushuo Chen, Zhipeng Chen, Jinhao Jiang, Ruiyang Ren, Yifan Li, Xinyu Tang, Zikang Liu, Peiyu Liu, Jian-Yun Nie, and Ji-Rong Wen. A survey of large language models, 2024.

[3] Sumit Kumar Dam, Choong Seon Hong, Yu Qiao, and Chaoning Zhang. A complete survey on llm-based ai chatbots, 2024.

[4] Aditi Singh. A survey of ai text-to-image and ai text-to-video generators. In 2023 4th International Conference on Artificial Intelligence, Robotics and Control (AIRC), pages 32–36, 2023.

[5] Aditi Singh, Abul Ehtesham, Gaurav Kumar Gupta, Nikhil Kumar Chatta, Saket Kumar, and Tala Talaei Khoei. Exploring prompt engineering: A systematic review with swot analysis, 2024.

[6] Lei Huang, Weijiang Yu, Weitao Ma, Weihong Zhong, Zhangyin Feng, Haotian Wang, Qianglong Chen, Weihua Peng, Xiaocheng Feng, Bing Qin, and Ting Liu. A survey on hallucination in large language models: Principles, taxonomy, challenges, and open questions. ACM Transactions on Information Systems, November 2024.

[7] Meng-Chieh Lee, Qi Zhu, Costas Mavromatis, Zhen Han, Soji Adeshina, Vassilis N. Ioannidis, Huzefa Rangwala, and Christos Faloutsos. Agent-g: An agentic framework for graph retrieval augmented generation, 2024.

[8] Penghao Zhao, Hailin Zhang, Qinhan Yu, Zhengren Wang, Yunteng Geng, Fangcheng Fu, Ling Yang, Wentao Zhang, Jie Jiang, and Bin Cui. Retrieval-augmented generation for ai-generated content: A survey, 2024.

[9] Zhengbao Jiang, Frank F. Xu, Luyu Gao, Zhiqing Sun, Qian Liu, Jane Dwivedi-Yu, Yiming Yang, Jamie Callan, and Graham Neubig. Active retrieval augmented generation, 2023.

[10] Yikun Han, Chunjiang Liu, and Pengfei Wang. A comprehensive survey on vector database: Storage and retrieval technique, challenge, 2023.

[11] Lei Wang, Chen Ma, Xueyang Feng, Zeyu Zhang, Hao Yang, Jingsen Zhang, Zhiyuan Chen, Jiakai Tang, Xu Chen, Yankai Lin, Wayne Xin Zhao, Zhewei Wei, and Jirong Wen. A survey on large language model based autonomous agents. Frontiers of Computer Science, 18(6), March 2024.

[12] Aditi Singh, Saket Kumar, Abul Ehtesham, Tala Talaei Khoei, and Deepshikha Bhati. Large language model-driven immersive agent. In 2024 IEEE World AI IoT Congress (AIIoT), pages 0619–0624, 2024.

[13] Matthew Renze and Erhan Guven. Self-reflection in llm agents: Effects on problem-solving performance, 2024.

[14] Xu Huang, Weiwen Liu, Xiaolong Chen, Xingmei Wang, Hao Wang, Defu Lian, Yasheng Wang, Ruiming Tang, and Enhong Chen. Understanding the planning of llm agents: A survey, 2024.

[15] Taicheng Guo, Xiuying Chen, Yaqi Wang, Ruidi Chang, Shichao Pei, Nitesh V. Chawla, Olaf Wiest, and Xiangliang Zhang. Large language model based multi-agents: A survey of progress and challenges, 2024.

[16] Chidaksh Ravuru, Sagar Srinivas Sakhinana, and Venkataramana Runkana. Agentic retrieval-augmented generation for time series analysis, 2024.

[17] Jie Huang and Kevin Chen-Chuan Chang. Towards reasoning in large language models: A survey, 2023.

[18] Boci Peng, Yun Zhu, Yongchao Liu, Xiaohe Bo, Haizhou Shi, Chuntao Hong, Yan Zhang, and Siliang Tang. Graph retrieval-augmented generation: A survey, 2024.

[19] Aditi Singh, Abul Ehtesham, Saifuddin Mahmud, and Jong-Hoon Kim. Revolutionizing mental health care through langchain: A journey with a large language model. In 2024 IEEE 14th Annual Computing and Communication Workshop and Conference (CCWC), pages 0073–0078, 2024.

[20] Gaurav Kumar Gupta, Aditi Singh, Sijo Valayakkad Manikandan, and Abul Ehtesham. Digital diagnostics: The potential of large language models in recognizing symptoms of common illnesses, 2024.

[21] Aditi Singh, Abul Ehtesham, Saket Kumar, Gaurav Kumar Gupta, and Tala Talaei Khoei. Encouraging responsible use of generative ai in education: A reward-based learning approach. In Tim Schlippe, Eric C. K. Cheng, and Tianchong Wang, editors, Artificial Intelligence in Education Technologies: New Development and Innovative Practices, pages 404–413, Singapore, 2025. Springer Nature Singapore.

[22] Yunfan Gao, Yun Xiong, Xinyu Gao, Kangxiang Jia, Jinliu Pan, Yuxi Bi, Yi Dai, Jiawei Sun, Meng Wang, and Haofen Wang. Retrieval-augmented generation for large language models: A survey, 2024.

[23] Vladimir Karpukhin, Barlas O˘guz, Sewon Min, Patrick Lewis, Ledell Wu, Sergey Edunov, Danqi Chen, and Wen tau Yih. Dense passage retrieval for open-domain question answering, 2020.

[24] Zeyu Zhang, Xiaohe Bo, Chen Ma, Rui Li, Xu Chen, Quanyu Dai, Jieming Zhu, Zhenhua Dong, and Ji-Rong Wen. A survey on the memory mechanism of large language model based agents, 2024.

[25] Zhibin Gou, Zhihong Shao, Yeyun Gong, Yelong Shen, Yujiu Yang, Nan Duan, and Weizhu Chen. Critic: Large language models can self-correct with tool-interactive critiquing, 2024.
[26] Aditi Singh, Abul Ehtesham, Saket Kumar, and Tala Talaei Khoei. Enhancing AI systems with agentic workflows patterns in large language model. In 2024 IEEE World AI IoT Congress (AIIoT), pages 527–532, 2024.

[27] DeepLearning.AI. How agents can improve LLM performance. [DeepLearning.AI](https://www.deeplearning.ai/the-batch/how-agents-can-improve-llm-performance/?ref=dl-staging-website.ghost.io), 2024. Accessed: 2025-01-13.

[28] Aman Madaan, Niket Tandon, Prakhar Gupta, Skyler Hallinan, Luyu Gao, Sarah Wiegreffe, Uri Alon, Nouha Dziri, Shrimai Prabhumoye, Yiming Yang, Shashank Gupta, Bodhisattwa Prasad Majumder, Katherine Hermann, Sean Welleck, Amir Yazdanbakhsh, and Peter Clark. Self-refine: Iterative refinement with self-feedback, 2023.

[29] Noah Shinn, Federico Cassano, Edward Berman, Ashwin Gopinath, Karthik Narasimhan, and Shunyu Yao. Reflexion: Language agents with verbal reinforcement learning, 2023.

[30] Weaviate Blog. What is agentic RAG? [Weaviate Blog](https://weaviate.io/blog/what-is-agentic-rag#:~:text=is%20Agentic%20RAG%3F-,%E2%80%8B,of%20the%20non%2Dagentic%20pipeline), 2024. Accessed: 2025-01-14.

[31] Shi-Qi Yan, Jia-Chen Gu, Yun Zhu, and Zhen-Hua Ling. Corrective retrieval augmented generation, 2024.

[32] LangGraph CRAG Tutorial. LangGraph CRAG: Contextualized retrieval-augmented generation tutorial. [LangGraph CRAG](https://langchain-ai.github.io/langgraph/tutorials/rag/langgraph_crag/). Accessed: 2025-01-14.

[33] Soyeong Jeong, Jinheon Baek, Sukmin Cho, Sung Ju Hwang, and Jong C. Park. Adaptive-RAG: Learning to adapt retrieval-augmented large language models through question complexity, 2024.

[34] LangGraph Adaptive RAG Tutorial. LangGraph adaptive RAG: Adaptive retrieval-augmented generation tutorial. [LangGraph Adaptive RAG](https://langchain-ai.github.io/langgraph/tutorials/rag/langgraph_adaptive_rag/). Accessed: 2025-01-14.

[35] Zhili Shen, Chenxin Diao, Pavlos Vougiouklis, Pascual Merita, Shriram Piramanayagam, Damien Graux, Dandan Tu, Zeren Jiang, Ruofei Lai, Yang Ren, and Jeff Z. Pan. GEAR: Graph-enhanced agent for retrieval-augmented generation, 2024.

[36] LlamaIndex. Introducing agentic document workflows. [LlamaIndex](https://www.llamaindex.ai/blog/introducing-agentic-document-workflows), 2025. Accessed: 2025-01-13.

[37] AWS Machine Learning Blog. How Twitch used agentic workflow with RAG on Amazon Bedrock to supercharge ad sales. [AWS Machine Learning Blog](https://aws.amazon.com/blogs/machine-learning/how-twitch-used-agentic-workflow-with-rag-on-amazon-bedrock-to-supercharge-ad-sales/), 2025. Accessed: 2025-01-13.

[38] LlamaCloud Demo Repository. Patient case summary workflow using LlamaCloud. [GitHub](https://github.com/run-llama/llamacloud-demo/blob/main/examples/document_workflows/patient_case_summary/patient_case_summary.ipynb), 2025. Accessed: 2025-01-13.

[39] LlamaCloud Demo Repository. Contract review workflow using LlamaCloud. [GitHub](https://github.com/run-llama/llamacloud-demo/blob/main/examples/document_workflows/contract_review/contract_review.ipynb), 2025. Accessed: 2025-01-13.

[40] LlamaCloud Demo Repository. Auto insurance claims workflow using LlamaCloud. [GitHub](https://github.com/run-llama/llamacloud-demo/blob/main/examples/document_workflows/auto_insurance_claims/auto_insurance_claims.ipynb), 2025. Accessed: 2025-01-13.

[41] LlamaCloud Demo Repository. Research paper report generation workflow using LlamaCloud. [GitHub](https://github.com/run-llama/llamacloud-demo/blob/main/examples/report_generation/research_paper_report_generation.ipynb), 2025. Accessed: 2025-01-13.

[42] LangGraph Agentic RAG Tutorial. LangGraph agentic RAG: Nodes and edges tutorial. [LangGraph Tutorial](https://langchain-ai.github.io/langgraph/tutorials/rag/langgraph_agentic_rag/#nodes-and-edges). Accessed: 2025-01-14.

[43] LlamaIndex Blog. Agentic RAG with LlamaIndex. [LlamaIndex Blog](https://www.llamaindex.ai/blog/agentic-rag-with-llamaindex-2721b8a49ff6). Accessed: 2025-01-14.

[44] Hugging Face Cookbook. Agentic RAG: Turbocharge your retrieval-augmented generation with query reformulation and self-query. [Hugging Face Cookbook](https://huggingface.co/learn/cookbook/en/agent_rag). Accessed: 2025-01-14.

[45] Qdrant Blog. Agentic RAG: Combining RAG with agents for enhanced information retrieval. [Qdrant Blog](https://qdrant.tech/articles/agentic-rag/). Accessed: 2025-01-14.

[46] OpenAI. Swarm: Lightweight multi-agent orchestration framework. [GitHub](https://github.com/openai/swarm). Accessed: 2025-01-14.

[47] LlamaIndex Documentation. Agentic RAG using Vertex AI. [LlamaIndex Documentation](https://docs.llamaindex.ai/en/stable/examples/agent/agentic_rag_using_vertex_ai/). Accessed: 2025-01-14.

[48] IBM Granite Community. Agentic RAG: AI agents with IBM Granite models. [GitHub](https://github.com/ibm-granite-community/granite-snack-cookbook/blob/main/recipes/AI-Agents/Agentic_RAG.ipynb). Accessed: 2025-01-14.

[49] Nandan Thakur, Nils Reimers, Andreas Rücklé, Abhishek Srivastava, and Iryna Gurevych. BEIR: A heterogeneous benchmark for zero-shot evaluation of information retrieval models, 2021.

[50] Payal Bajaj, Daniel Campos, Nick Craswell, Li Deng, Jianfeng Gao, Xiaodong Liu, Rangan Majumder, Andrew McNamara, Bhaskar Mitra, Tri Nguyen, Mir Rosenberg, Xia Song, Alina Stoica, Saurabh Tiwary, and Tong Wang. MS MARCO: A human-generated machine reading comprehension dataset, 2018.

[51] Nick Craswell, Bhaskar Mitra, Emine Yilmaz, Daniel Campos, Jimmy Lin, Ellen M. Voorhees, and Ian Soboroff. Overview of the TREC 2022 deep learning track. In Text Retrieval Conference (TREC), March 2023.

[52] Harsh Trivedi, Niranjan Balasubramanian, Tushar Khot, and Ashish Sabharwal. Musique: Multihop questions via single-hop question composition, 2022.

[53] Xanh Ho, Anh-Khoa Duong Nguyen, Saku Sugawara, and Akiko Aizawa. Constructing a multi-hop QA dataset for comprehensive evaluation of reasoning steps, 2020.

[54] Zhilin Yang, Peng Qi, Saizheng Zhang, Yoshua Bengio, William W. Cohen, Ruslan Salakhutdinov, and Christopher D. Manning. HotpotQA: A dataset for diverse, explainable multi-hop question answering, 2018.

[55] Robert Friel, Masha Belyi, and Atindriyo Sanyal. RAGBench: Explainable benchmark for retrieval-augmented generation systems, 2024.

[56] David Rau, Hervé Déjean, Nadezhda Chirkova, Thibault Formal, Shuai Wang, Vassilina Nikoulina, and Stéphane Clinchant. BERGEN: A benchmarking library for retrieval-augmented generation, 2024.

[57] Jiajie Jin, Yutao Zhu, Xinyu Yang, Chenghao Zhang, and Zhicheng Dou. FlashRAG: A modular toolkit for efficient retrieval-augmented generation research, 2024.

[58] Costas Mavromatis and George Karypis. GNN-RAG: Graph neural retrieval for large language model reasoning, 2024.

[59] Tom Kwiatkowski, Jennimaria Palomaki, Olivia Redfield, Michael Collins, Ankur Parikh, Chris Alberti, Danielle Epstein, Illia Polosukhin, Jacob Devlin, Kenton Lee, Kristina Toutanova, Llion Jones, Matthew Kelcey, Ming-Wei Chang, Andrew M. Dai, Jakob Uszkoreit, Quoc Le, and Slav Petrov. Natural Questions: A benchmark for question answering research. Transactions of the Association for Computational Linguistics, 7:452–466, 2019.

[60] Mandar Joshi, Eunsol Choi, Daniel S. Weld, and Luke Zettlemoyer. TriviaQA: A large scale distantly supervised challenge dataset for reading comprehension, 2017.

[61] Pranav Rajpurkar, Jian Zhang, Konstantin Lopyrev, and Percy Liang. SQuAD: 100,000+ questions for machine comprehension of text, 2016.

[62] Jonathan Berant, Andrew K. Chou, Roy Frostig, and Percy Liang. Semantic parsing on Freebase from question-answer pairs. In Conference on Empirical Methods in Natural Language Processing, 2013.

[63] Alex Mallen, Akari Asai, Victor Zhong, Rajarshi Das, Daniel Khashabi, and Hannaneh Hajishirzi. When not to trust language models: Investigating effectiveness of parametric and non-parametric memories. In Anna Rogers, Jordan Boyd-Graber, and Naoaki Okazaki, editors, Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers), pages 9802–9822, Toronto, Canada, July 2023. Association for Computational Linguistics.

[64] Angela Fan, Yacine Jernite, Ethan Perez, David Grangier, Jason Weston, and Michael Auli. ELI5: Long form question answering, 2019.

[65] Tomáš Kočiský, Jonathan Schwarz, Phil Blunsom, Chris Dyer, Karl Moritz Hermann, Gábor Melis, and Edward Grefenstette. The NarrativeQA reading comprehension challenge, 2017.

[66] Ivan Stelmakh, Yi Luan, Bhuwan Dhingra, and Ming-Wei Chang. ASQA: Factoid questions meet long-form answers, 2023.

[67] Ming Zhong, Da Yin, Tao Yu, Ahmad Zaidi, Mutethia Mutuma, Rahul Jha, Ahmed Hassan Awadallah, Asli Celikyilmaz, Yang Liu, Xipeng Qiu, and Dragomir Radev. QMSum: A new benchmark for query-based multi-domain meeting summarization, June 2021.

[68] Pradeep Dasigi, Kyle Lo, Iz Beltagy, Arman Cohan, Noah A. Smith, and Matt Gardner. A dataset of information-seeking questions and answers anchored in research papers. In Kristina Toutanova, Anna Rumshisky, Luke Zettlemoyer, Dilek Hakkani-Tur, Iz Beltagy, Steven Bethard, Ryan Cotterell, Tanmoy Chakraborty, and Yichao Zhou, editors, Proceedings of the 2021 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, pages 4599–4610, Online, June 2021. Association for Computational Linguistics.

[69] Timo Möller, Anthony Reina, Raghavan Jayakumar, and Malte Pietsch. COVID-QA: A question answering dataset for COVID-19. In ACL 2020 Workshop on Natural Language Processing for COVID-19 (NLP-COVID), 2020.

[70] Xidong Wang, Guiming Hardy Chen, Dingjie Song, Zhiyi Zhang, Zhihong Chen, Qingying Xiao, Feng Jiang, Jianquan Li, Xiang Wan, Benyou Wang, and Haizhou Li. CMB: A comprehensive medical benchmark in Chinese, 2024.

[71] Richard Yuanzhe Pang, Alicia Parrish, Nitish Joshi, Nikita Nangia, Jason Phang, Angelica Chen, Vishakh Padmakumar, Johnny Ma, Jana Thompson, He He, and Samuel R. Bowman. Quality: Question answering with long input texts, yes!, 2022.

[72] Alon Talmor, Jonathan Herzig, Nicholas Lourie, and Jonathan Berant. CommonsenseQA: A question answering challenge targeting commonsense knowledge. In Jill Burstein, Christy Doran, and Thamar Solorio, editors, Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long and Short Papers), pages 4149–4158, Minneapolis, Minnesota, June 2019. Association for Computational Linguistics.

[73] Xiaoxin He, Yijun Tian, Yifei Sun, Nitesh V. Chawla, Thomas Laurent, Yann LeCun, Xavier Bresson, and Bryan Hooi. G-Retriever: Retrieval-augmented generation for textual graph understanding and question answering, 2024.

[74] Sha Li, Heng Ji, and Jiawei Han. Document-level event argument extraction by conditional generation, 2021.

[75] Seth Ebner, Patrick Xia, Ryan Culkin, Kyle Rawlins, and Benjamin Van Durme. Multi-sentence argument linking, 2020.

[76] Emily Dinan, Stephen Roller, Kurt Shuster, Angela Fan, Michael Auli, and Jason Weston. Wizard of Wikipedia: Knowledge-powered conversational agents, 2019.

[77] Hongru Wang, Minda Hu, Yang Deng, Rui Wang, Fei Mi, Weichao Wang, Yasheng Wang, Wai-Chung Kwan, Irwin King, and Kam-Fai Wong. Large language models as source planner for personalized knowledge-grounded dialogue, 2023.

[78] Xinchao Xu, Zhibin Gou, Wenquan Wu, Zheng-Yu Niu, Hua Wu, Haifeng Wang, and Shihang Wang. Long time no see! Open-domain conversation with long-term persona memory, 2022.

[79] Tsung-Hsien Wen, Milica Gašić, Nikola Mrkšić, Lina M. Rojas-Barahona, Pei-Hao Su, Stefan Ultes, David Vandyke, and Steve Young. Conditional generation and snapshot learning in neural dialogue systems. In Proceedings of the 2016 Conference on Empirical Methods in Natural Language Processing, pages 2153–2162, Austin, Texas, November 2016. Association for Computational Linguistics.

[80] Ruining He and Julian McAuley. Ups and downs: Modeling the visual evolution of fashion trends with one-class collaborative filtering. In Proceedings of the 25th International Conference on World Wide Web, WWW ’16, page 507–517, Republic and Canton of Geneva, CHE, 2016. International World Wide Web Conferences Steering Committee.

[81] Rowan Zellers, Ari Holtzman, Yonatan Bisk, Ali Farhadi, and Yejin Choi. HellaSwag: Can a machine really finish your sentence? In Anna Korhonen, David Traum, and Lluís Màrquez, editors, Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics, pages 4791–4800, Florence, Italy, July 2019. Association for Computational Linguistics.

[82] Seungone Kim, Se June Joo, Doyoung Kim, Joel Jang, Seonghyeon Ye, Jamin Shin, and Minjoon Seo. The CoT collection: Improving zero-shot and few-shot learning of language models via chain-of-thought fine-tuning, 2023.

[83] Amrita Saha, Vardaan Pahuja, Mitesh M. Khapra, Karthik Sankaranarayanan, and Sarath Chandar. Complex sequential question answering: Towards learning to converse over linked question answer pairs with a knowledge graph, 2018.

[84] James Thorne, Andreas Vlachos, Christos Christodoulopoulos, and Arpit Mittal. FEVER: A large-scale dataset for fact extraction and verification. In Marilyn Walker, Heng Ji, and Amanda Stent, editors, Proceedings of the 2018 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long Papers), pages 809–819, New Orleans, Louisiana, June 2018. Association for Computational Linguistics.

[85] Neema Kotonya and Francesca Toni. Explainable automated fact-checking for public health claims, 2020.

[86] Mor Geva, Daniel Khashabi, Elad Segal, Tushar Khot, Dan Roth, and Jonathan Berant. Did Aristotle use a laptop? A question answering benchmark with implicit reasoning strategies, 2021.

[87] Hiroaki Hayashi, Prashant Budania, Peng Wang, Chris Ackerson, Raj Neervannan, and Graham Neubig. WikiASP: A dataset for multi-domain aspect-based summarization, 2020.

[88] Shashi Narayan, Shay B. Cohen, and Mirella Lapata. Don’t give me the details, just the summary! Topic-aware convolutional neural networks for extreme summarization, 2018.

[89] Richard Socher, Alex Perelygin, Jean Wu, Jason Chuang, Christopher D. Manning, Andrew Ng, and Christopher Potts. Recursive deep models for semantic compositionality over a sentiment treebank. In David Yarowsky, Timothy Baldwin, Anna Korhonen, Karen Livescu, and Steven Bethard, editors, Proceedings of the 2013 Conference on Empirical Methods in Natural Language Processing, pages 1631–1642, Seattle, Washington, USA, October 2013. Association for Computational Linguistics.

[90] Sourav Saha, Jahedul Alam Junaed, Maryam Saleki, Arnab Sen Sharma, Mohammad Rashidujjaman Rifat, Mohamed Rahouti, Syed Ishtiaque Ahmed, Nabeel Mohammed, and Mohammad Ruhul Amin. Vio-lens: A novel dataset of annotated social network posts leading to different forms of communal violence and its evaluation. In Firoj Alam, Sudipta Kar, Shammur Absar Chowdhury, Farig Sadeque, and Ruhul Amin, editors, Proceedings of the First Workshop on Bangla Language Processing (BLP-2023), pages 72–84, Singapore, December 2023. Association for Computational Linguistics.

[91] Hamel Husain, Ho-Hsiang Wu, Tiferet Gazit, Miltiadis Allamanis, and Marc Brockschmidt. CodeSearchNet challenge: Evaluating the state of semantic code search, 2020.

[92] Nandan Thakur, Luiz Bonifacio, Xinyu Zhang, Odunayo Ogundepo, Ehsan Kamalloo, David Alfonso-Hermelo, Xiaoguang Li, Qun Liu, Boxing Chen, Mehdi Rezagholizadeh, and Jimmy Lin. "Knowing when you don’t know": A multilingual relevance assessment dataset for robust retrieval-augmented generation, 2024.

[93] Stephen Merity, Caiming Xiong, James Bradbury, and Richard Socher. Pointer sentinel mixture models, 2016.

[94] Karl Cobbe, Vineet Kosaraju, Mohammad Bavarian, Mark Chen, Heewoo Jun, Lukasz Kaiser, Matthias Plappert, Jerry Tworek, Jacob Hilton, Reiichiro Nakano, Christopher Hesse, and John Schulman. Training verifiers to solve math word problems, 2021.

[95] Ralf Steinberger, Bruno Pouliquen, Anna Widiger, Camelia Ignat, Tomaž Erjavec, Dan Tufiș, and Dániel Varga. The JRC-Acquis: A multilingual aligned parallel corpus with 20+ languages. In Nicoletta Calzolari, Khalid Choukri, Aldo Gangemi, Bente Maegaard, Joseph Mariani, Jan Odijk, and Daniel Tapias, editors, Proceedings of the Fifth International Conference on Language Resources and Evaluation (




---

## How to Cite

If you find this work useful in your research, please cite:

```bibtex
@article{agenticRAG,
  title={Agentic Retrieval-Augmented Generation (RAG): A Comprehensive Survey},
  author={Your Name and Co-Authors},
  year={2024},
  journal={ArXiv},
  url={https://github.com/YourRepo/AgenticRAG-Survey}
}
