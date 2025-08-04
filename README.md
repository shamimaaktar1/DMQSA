<p align="center">
    <img src="https://github.com/user-attachments/assets/a98339cc-f51d-4d03-99a0-49074b899d37" alt="Logo" width="180" height="230" />
</p>

<h2 align="center">Decision Models for Selecting Architecture Patterns and Strategies in Quantum Software Systems</h2>

<p align="left">
  This is the replication package for the paper: "Decision Models for Selecting Architecture Patterns and Strategies in Quantum Software Systems", including the dataset, figures of decision models, and so on (see the description below).
</p>

## File Organization

1. `data_for_constructing_the_decision_models.xlsx` contains the information about i) Selected  GitHub Projects, ii) Selected Stack Exchange Sites, iii) Selected Databases, iv) Selected GitHub Issues & Pull Requests (PR), v) Selected Stack Exchange Posts, vi) Selected Studies, vii) GitHub Raw Data, viii) Stack Exchange Raw Data, ix) Scientific Studies Raw Data, x) Pattern & Strategy Impact, and xi) Selected Patterns & Strategies
2.   `interview_data.xlsx` contains the information about i) Demographic Information, ii) Practitioner Feedback on the Communication Decision Model, iii) Practitioner Feedback on the Decomposition Decision Model, iv) Practitioner Feedback on the Data processing Decision Model, v) Practitioner Feedback on the Fault Tolerance Decision Model, vi) Practitioner Feedback on the Integration and Optimization Decision Model, and vii) Practitioner Feedback on the Algorithm Implementation Decision Model

## Experiment Replication Steps

This research paper is divided into three main phases.

- [Stage 1: Research Design](#stage-1-research-design)
  - [Identifying Quantum Patterns and Strategies](#identifying-quantum-patterns-and-strategies)
  - [Modeling Decision Models](#modeling-decision-models)
  - [Evaluating Decision Models](#evaluating-decision-models)

- [Stage 2: Decision Models](#stage-2-decision-models)
  - [Decision Model for Communication](#decision-model-for-communication)
  - [Decision Model for Decomposition](#decision-model-for-decomposition)
  - [Decision Model for Data Processing](#decision-model-for-data-processing)
  - [Decision Model for Fault Tolerance](#decision-model-for-fault-tolerance)
  - [Decision Model for Integration and Optimization](#decision-model-for-integration-and-optimization)
  - [Decision Model for Algorithm Implementation](#decision-model-for-algorithm-implementation)
 
- [Stage 3: Evaluation](#stage-3-evaluation)
  - [Participant Demographics and Professional Background](#participant-demographics-and-professional-background)
  - [Practitioner Feedback on Decision Models](#practitioner-feedback-on-decision-models)

---

### Stage 1: Research Design

<p>
The decision models were explicitly crafted for four critical areas of quantum software design: structural abstraction, communication, integration and optimization, and data processing. These areas were chosen because they are fundamental to addressing critical design, implementation, integration, and data management challenges.
</p>
The research method is described below and represented in the picture below:
<br>
<br>

<p align="center">
   <img src="https://github.com/user-attachments/assets/c4ebd8fc-b7ce-4547-ba3e-41ab197e0032" alt="Research Process"  width="650" height="600">
</p>

<p align="center"><b>Figure 1:</b> Overview of the research process</p>

---

#### Identifying Quantum Patterns and Strategies

<p>To comprehensively support the development of decision models for quantum software architecture, we systematically integrated the findings from both the mining study (GitHub issues and Stack Exchange posts) and the systematic literature review. This process resulted in the identification of 372 architecture patterns and strategies: 162 from the mining study, comprising 145 from 121 GitHub issues and pull requests, 17 from 13 Stack Exchange posts, and 210 from 92 peer-reviewed scientific studies. After removing duplicates and semantically consolidating similar entries, we derived a final set of 63 unique architecture patterns and strategies, which were categorized into six key design areas in quantum software systems: 1) 18 for Communication, 2) 7 for Decomposition, 3) 12 for Data Processing, 4) 8 for Fault Tolerance, 5) 9 for Integration and Optimization, and 6) 9 for Algorithm Implementation.
</p>

---

#### Modeling Decision Models

To model the decision-making process for selecting architectural patterns and strategies in quantum software systems, we adopted the Business Process Model and Notation (BPMN). The following elements are used in each decision model:

1. A **grey box** represents a specific design area within quantum software systems (e.g., Communication, Decomposition).
2. A **circle** marks the **starting point** of the decision process.
3. An **Inclusive Gateway** allows multiple outgoing paths to be activated based on specific conditions.
4. An **Exclusive Gateway** permits only one outgoing path to proceed based on a selected condition.
5. A **Parallel Gateway** triggers all outgoing paths simultaneously to represent concurrent execution.
6. **Rounded rectangles** depict architectural patterns and strategies relevant to the design area.
7. A **plus sign (+)** indicates a *quality attribute* positively influenced by the associated pattern or strategy.
8. A **minus sign (-)** indicates a *quality attribute* negatively impacted by the pattern or strategy.
9. An **octagon** connected by a **dashed arrow** to a pattern denotes a constraint applied to that pattern.
10. A **double-headed arrow (⇉)** pointing in the same direction represents a *complements* relationship between two patterns or strategies.
11. A **single-headed arrow (→)** indicates a *conditional flow* between elements in the decision process.

This modeling structure ensures a clear, traceable, and standardized representation of decision flows, helping practitioners evaluate trade-offs and make informed architectural decisions in quantum software systems.

<br>

<p align="center">
   <img src="https://github.com/user-attachments/assets/4ca46ea6-5987-4098-8bdd-ebbb30c33a34" alt="Model and Notation (BPMN)"  width="650" height="210">
</p>

<p align="center"><b>Figure 2:</b> Notations used in the decision models</p>

---

#### Evaluating Decision Models

To evaluate the proposed decision models, we conducted semi-structured interviews with 16 quantum software practitioners from eight countries. Participants were selected through GitHub, professional platforms (e.g., LinkedIn, Facebook), and personal networks. Participants were selected through GitHub, professional platforms (e.g., LinkedIn, Facebook), and personal networks. Invitations to participate were posted in several professional groups, providing links to the [interview questionnaire](https://tinyurl.com/bdcvzjjb) and a supplementary document containing [architectural pattern examples](https://tinyurl.com/2fwcbkmh).  The details of the groups where the invitations were shared are listed in **Table 1**. The interview guide, structured into seven sections, was designed to evaluate six decision models across key design areas and to collect both quantitative and qualitative feedback. Inclusion and exclusion criteria were applied to ensure the quality and relevance of responses. All interviews were transcribed, coded, and analyzed using descriptive statistics and grounded theory methods. 

This evaluation enabled a comprehensive assessment of the models’ *usefulness*, *correctness*, *completeness*, and *understandability*, providing practitioner-driven insights for refining the decision models.
. The interview guide, structured into seven sections, assessed six decision models across core design areas and collected both quantitative and qualitative insights. Inclusion and exclusion criteria ensured high-quality responses. Interviews were transcribed, coded, and analyzed using descriptive statistics and grounded theory methods. This evaluation helped assess the models’ *usefulness*, *correctness*, *completeness*, and *understandability*, offering practitioner-driven insights to refine the decision models.


<p align="center"><b>Table 1:</b> Quantum software practitioners’ social and professional platforms used for interview invitations</p>

<font size="1">

| #  | Group Name                                                                 | URL                                             | Group Members | Platform |
|----|-----------------------------------------------------------------------------|-------------------------------------------------|---------------|----------|
| 1  | Quantum Computing                                                           | [Link](https://tinyurl.com/2uacpcbz)            | 22,277        | LinkedIn |
| 2  | Quantum Mechanics / Physics / Theory / Leap / Computing Information Science | [Link](https://tinyurl.com/47hhn7cr)            | 12,805        | LinkedIn |
| 3  | European Quantum Computing Applications Community                           | [Link](https://tinyurl.com/ynu68vh9)             | 9,108         | LinkedIn |
| 4  | Quantum Computing (IBM)                                                     | [Link](https://tinyurl.com/2phtyu7h)            | 7,655         | LinkedIn |
| 5  | Quantum Computing Technology                                                | [Link](https://tinyurl.com/5e6ujnmm)            | 7,091         | LinkedIn |
| 6  | Quantum Computing and AI Professionals                                      | [Link](https://tinyurl.com/6van9fbh)            | 2,900         | LinkedIn |
| 7  | Quantum Technologies Opportunities Network                                   | [Link](https://tinyurl.com/mrxv6wpc)            | 1,328         | LinkedIn |
| 8  | Artificial Intelligence and Quantum Computing Network - Next Realm AI       | [Link](https://tinyurl.com/yckafcwp)            | 997           | LinkedIn |
| 9  | Quantum Computing QC - A Tachyon Knowledge Initiative                       | [Link](https://tinyurl.com/ywk3tpjv)            | 881           | LinkedIn |
| 10 | Quantum Information CyberSecurity Computing I Computer, Simulation & Cryptography barcelonaqbit.com | [Link](https://tinyurl.com/2kt6byr3)            | 741           | LinkedIn |
| 11 | Quantum Science Communication & Outreach (QSCO)                             | [Link](https://tinyurl.com/yvmt6s93)            | 577           | LinkedIn |
| 12 | Quantum Computing and Machine Learning                                      | [Link](https://tinyurl.com/5eyuj6je)            | 484           | LinkedIn |
| 13 | von Neumann Forum - Quantum Algorithms, Quantum Computing and Quantum Machine Learning | [Link](https://tinyurl.com/ycya28x8)            | 366           | LinkedIn |
| 14 | Quantum Software Engineering                                                | [Link](https://tinyurl.com/ep8d42tm)            | 47            | LinkedIn |
| 15 | Quantum Enlightenment                                                        | [Link](https://tinyurl.com/2vet6yej)            | 2,000         | Facebook |
| 16 | Software Architects Discussions                                              | [Link](https://tinyurl.com/2yubyzur)            | 39,200        | Facebook |
| 17 | Quantum AI                                                                  | [Link](https://tinyurl.com/ms22u95v)            | 8,800         | Facebook |

</font>

### Stage 2: Decision Models

<p>
We proposed a set of decision models for selecting patterns and strategies in six critical areas of quantum software system design: <strong>Communication</strong>, <strong>Decomposition</strong>, <strong>Data Processing</strong>, <strong>Fault Tolerance</strong>, <strong>Integration and Optimization</strong>, and <strong>Algorithm Implementation</strong>. These models are developed based on insights gathered from analyzing real-world development discussions in GitHub issues and Stack Exchange posts. They aim to guide practitioners in addressing design challenges by providing structured pathways to select suitable architectural patterns and strategies while balancing relevant quality trade-offs.
</p>

---

#### Decision Model for Communication

The decision model for communication in quantum software systems provides a structured framework to guide practitioners in selecting architecture patterns and strategies for both quantum-to-quantum and quantum-to-classical communication. Informed by mining studies and literature, it maps communication scenarios to architectural solutions using Inclusive, Exclusive, and Parallel Gateways. The model supports diverse communication needs—ranging from managing hybrid workflows (e.g., **Quantum API Gateway**, **Workflow Orchestration**) to secure long-distance quantum networking (e.g., **Entanglement Distribution**, **Teleportation**, **QKD Protocols**). It distinguishes between **Connection-Oriented** and **Connectionless Strategies**, and includes broadcasting, layered architectures, and performance-enhancing solutions such as **Quantum Burst Communication** and **Entanglement-Assisted Channels**. Each pattern is annotated with its associated trade-offs across key quality attributes (QAs) such as *Security*, *Scalability*, *Modularity*, and *Performance*, enabling informed, context-sensitive decisions for building robust quantum communication systems.

<br>

<p align="center">
   <img src="https://github.com/user-attachments/assets/ce1663e1-1d5f-4398-821e-41246e8cf7d0" alt="Decision Model for Communication"  width="650" height="800">
</p>

<p align="center"><b>Figure 3:</b> Decision model for selecting architecture patterns and strategies for communication</p>

---

#### Decision Model for Decomposition

This decision model provides structured guidance for selecting appropriate decomposition strategies in quantum software systems. It uses gateways to navigate multiple paths based on system goals—such as separating quantum-classical logic, enforcing architectural layers, or aligning with functional or business capabilities. The model incorporates patterns like **Quantum-Classic Split**, **Quantum Microservices**, **Layered Architecture**, and others, each selected based on specific design contexts and targeted QAs such as *Scalability*, *Maintainability*, *Performance*, and *Modularity*. By mapping conditions to pattern impacts, the model ensures that decomposition decisions are tailored to the unique structural and operational needs of quantum-classical hybrid systems.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/abf6aca3-9bb2-4a58-b5ba-ec9340e37977" alt="Decision Model for Decomposition"  width="650" height="450">
</p>

<p align="center"><b>Figure 4:</b> Decision model for selecting architecture patterns and strategies for decomposition</p>

---

#### Decision Model for Data Processing

This decision model provides a structured approach to selecting suitable architecture patterns and encoding strategies for quantum data processing. It leverages gateways to guide decisions based on workload characteristics, data transformation needs, and QAs trade-offs. The model includes patterns such as **Pipe and Filter**, **Consumer**, and **Quantum Mediator Wrapper** for managing quantum-classical workflows, dynamic resource allocation, and heterogeneous data integration. Encoding strategies like **Basis**, **Amplitude**, and **Angle Encoding** support *Flexible* representation of classical data in quantum states. The model also incorporates advanced components like **Quantum Associative Memory** and **QRAM** to address retrieval and *Scalability* concerns. By aligning each path with specific QAs such as *Performance*, *Modularity*, *Scalability*, and *Interoperability* the model aids practitioners in building efficient and adaptable quantum software systems.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/477289f6-a289-4a35-8336-00433a5365f1" alt="Decision Model for Data Processing"  width="650" height="550">
</p>

<p align="center"><b>Figure 5:</b> Decision model for selecting architecture patterns and strategies for data processing</p>

---

#### Decision Model for Fault Tolerance

This decision model guides quantum software developers in selecting fault tolerance strategies that align with specific system needs such as detection, correction, and adaptability. Using a structured flow of Inclusive and Exclusive Gateways, the model evaluates multiple conditions—component failure, noisy gates, readout errors, or runtime adaptation—and maps them to suitable architectural patterns. It includes classical strategies like **Sparing**, **Voting**, and **Comparison** for redundancy and detection, as well as quantum-specific solutions such as **Error Correction**, **Readout Error Mitigation**, **Gate Error Mitigation**,  **Decorator Design**, and **Quantum Patterns of Behavior (qPoB)**. Each path is aligned with trade-offs in QAs like *Reliability*, *Fault Recovery*, *Scalability*, and *Complexity*, enabling systematic fault-resilient design in quantum software systems.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/16e0d7b8-76f9-4789-bb60-80f9143d2a42" alt="Decision Model for Fault Tolerance"  width="650" height="550">
</p>

<p align="center"><b>Figure 6:</b> Decision model for selecting architecture patterns and strategies for fault tolerance</p>

---

#### Decision Model for Integration and Optimization

This decision model guides quantum software developers in selecting architecture patterns that address system-wide integration and optimization needs. Using structured gateways, it supports decisions across three main areas: integrating diverse quantum-classical components, optimizing quantum processes, and orchestrating scalable, service-based architectures. Patterns such as **Integration Pattern**, **Prototype Design Pattern**, **Quantum Broadcast Pattern**, **Transformer Design Pattern**, and **Quantum Service-Oriented Architecture** are selected based on specific QAs like *Performance*, *Scalability*, *Modularity*, and *Interoperability*. The model balances trade-offs by providing tailored paths for hybrid coordination, parallel execution, service composition, and deployment flexibility.



<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/316c8c90-ec53-44b0-9842-9e4887ed3bc2" alt="Decision Model for Integration and Optimization"  width="650" height="500">
</p>

<p align="center"><b>Figure 7:</b> Decision model for selecting architecture patterns and strategies for integration and optimization</p>

---

#### Decision Model for Algorithm Implementation

The decision model for algorithm implementation in quantum software systems provides a structured approach for selecting suitable architectural patterns based on specific integration needs, modularization strategies, and target QAs. It begins with hybrid execution concerns, such as coordinating classical and quantum components—using patterns like **Hybrid Module**, **Quantum-Classic Split**, and **Classical-Quantum Interface**. The model then guides practitioners through the design quantum algorithm module via **Quantum Module** and **Quantum Module Template**, and optimization strategies like **Qubit Gate Pattern**, **Brickwork Pattern**, and **Template-Matching Pattern**. Finally, for device *Compatibility* and *Portability*, the **Quantum Circuit Translator pattern** is applied. Using inclusive, exclusive, and parallel gateways, the model helps balance trade-offs across key QAs such as *Reusability*, *Modularity*, *Interoperability*, and *Performance* to enable effective and maintainable quantum algorithm development.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/3e17d951-b6b2-4e52-bade-407e94c5ce14" alt="Decision Model for Algorithm Implementation"  width="650" height="400">
</p>

<p align="center"><b>Figure 8:</b> Decision model for selecting architecture patterns and strategies for algorithm implementation</p>

---

### Stage 3: Evaluation
<p>
To evaluate the proposed decision models, we conducted semi-structured interviews with 16 practitioners using a standardized <a href="https://tinyurl.com/bdcvzjjb">interview questionnaire</a>. The results of this evaluation are organized into two parts: (1) participant demographics and professional background, and (2) evaluation of the decision models with respect to familiarity, understandability, and correctness.
</p>

---

### Participant Demographics and Professional Background

<p>
To evaluate the decision models, we conducted semi-structured interviews with 16 practitioners from Asia, Africa, and Europe. Most participants had 6–10 years of experience in software development, and 2–10 years in quantum software development. Their roles ranged from researchers and developers to physicists and project managers, reflecting the interdisciplinary nature of the field. They were also involved in various quantum domains such as cryptography, AI/ML, optimization, simulation, and healthcare, often contributing to multiple domains simultaneously.
</p>
<p align="center">
   <img src="https://github.com/user-attachments/assets/ff749afe-6ff6-4121-ac6c-90a13455c6a6" alt="Demographic details of the interview participants"  width="600" height="450">
</p>

<p align="center"><b>Figure 9:</b> Demography details of interviewed practitioners</p>


---


### Practitioner Feedback on Decision Models

<p>
Practitioners generally reported high familiarity with the architectural patterns and strategies in the six proposed decision models. They found the models understandable, well-structured, and easy to apply in practice. All six models were considered sufficient for supporting architectural decisions in quantum software systems. Suggestions included adding more explicit trade-offs, clarifying relationships between patterns and QAs, and improving directional guidance. These inputs were incorporated into updated versions of the models.
</p>

<p align="center">
   <img src="https://github.com/user-attachments/assets/ca31f126-7c9e-44ca-8baf-04b0321209ea" alt="Overview of practitioners’ responses for familiarity, understandability, and completeness of the decision models"  width="600" height="400">
</p>

<p align="center"><b>Figure 10:</b> Overview of practitioners’ responses for familiarity, understandability, and completeness of the
decision models</p>


