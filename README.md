<p align="center">
    <img src="https://github.com/user-attachments/assets/a98339cc-f51d-4d03-99a0-49074b899d37" alt="Logo" width="180" height="230" />
</p>

<h2 align="center">Decision Models for Selecting Architecture Patterns and Strategies in Quantum Software Systems</h2>

<p align="left">
  This is the replication package for the paper: "Decision Models for Selecting Architecture Patterns and Strategies in Quantum Software Systems", including the dataset, figures of decision models, and so on (see the description below).
</p>

## File Organization


1. `Interview data.xlsx` contains the information about i) Demographic Information, ii) Practitioner Feedback on the Communication Decision Model, iii) Practitioner Feedback on the Decomposition Decision Model, iv) Practitioner Feedback on the Data processing Decision Model, v) Practitioner Feedback on the Fault Tolerance Decision Model, vi)  Practitioner Feedback on the Integration and Optimization Decision Model, and vii) Practitioner Feedback on the Algorithm Implementation Decision Model
2. `Data for constructing the decision models.xlsx` contains the information about i) Selected  GitHub Projects, ii) Selected Stack Exchange Sites, iii) Selected Databases, iv) Selected GitHub Issues & Pull Requests (PR), v) Selected Stack Exchange Posts, vi) Selected Studies, vii) GitHub Raw Data, viii) Stack Exchange Raw Data, ix) Scientific Studies Raw Data, x)Pattern & Strategy Impact, and xi) Selected Patterns & Strategies


## Experiment Replication Steps

This research paper is divided into three main phases.

- [Stage 1: Research Design](#research-design)
  - [Identifying Quantum Patterns and Strategies](#identifying-quantum-patterns-and-strategies)
  - [Modeling Decision Models](#modeling-decision-models)
  - [Evaluating Decision Models](#evaluating-decision-models)

- [Stage 2: Decision Models](#decision-models)
  - [Decision Model for Communication](#decision-model-for-communication)
  - [Decision Model for Decomposition](#decision-model-for-decomposition)
  - [Decision Model for Data Processing](#decision-model-for-data-processing)
  - [Decision Model for Fault Tolerance](#decision-model-for-fault-tolerance)
  - [Decision Model for Integration and Optimization](#decision-model-for-integration-and-optimization)
  - [Decision Model for Algorithm Implementation](#decision-model-for-algorithm-implementation)
 
- [Stage 3: Evaluation of Decision Models](#evaluation-of-decision-models)
  - [Participant Demographics and Professional Background](#participant-demographics-and-professional-background)
  - [Practitioner Feedback on Decision Models](#practitioner-feedback-on-decision-models)



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



#### Identifying Quantum Patterns and Strategies

<p>To comprehensively support the development of decision models for quantum software architecture, we systematically integrated the findings from both the mining study (GitHub issues and Stack Exchange posts) and the systematic literature review. This process resulted in the identification of 372 architecture patterns and strategies: 162 from the mining study, comprising 145 from 121 GitHub issues and pull requests, 17 from 13 Stack Exchange posts, and 210 from 92 peer-reviewed scientific studies. After removing duplicates and semantically consolidating similar entries, we derived a final set of 63 unique architecture patterns and strategies, which were categorized into six key design areas in quantum software systems: 1) 18 for Communication, 2) 7 for Decomposition, 3) 12 for Data Processing, 4) 8 for Fault Tolerance, 5) 9 for Integration and Optimization, and 6) 9 for Algorithm Implementation.
</p>


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

#### Evaluating Decision Models

To evaluate the proposed decision models, we conducted semi-structured interviews with 16 quantum software practitioners from eight countries, selected via GitHub, professional platforms (e.g., LinkedIn, Facebook), and personal networks. Participants received a questionnaire and a supplementary document with architectural pattern examples in advance. The interview guide, structured into seven sections, assessed six decision models across core design areas and collected both quantitative and qualitative insights. Inclusion and exclusion criteria ensured high-quality responses. Interviews were transcribed, coded, and analyzed using descriptive statistics and grounded theory methods. This evaluation helped assess the models’ *usefulness*, *correctness*, *completeness*, and *understandability*, offering practitioner-driven insights to refine the decision models.


### Stage 2: Decision Models

<p>
We proposed a set of decision models for selecting patterns and strategies in six critical areas of quantum software system design: <strong>Communication</strong>, <strong>Decomposition</strong>, <strong>Data Processing</strong>, <strong>Fault Tolerance</strong>, <strong>Integration and Optimization</strong>, and <strong>Algorithm Implementation</strong>. These models are developed based on insights gathered from analyzing real-world development discussions in GitHub issues and Stack Exchange posts. They aim to guide practitioners in addressing design challenges by providing structured pathways to select suitable architectural patterns and strategies while balancing relevant quality trade-offs.
</p>

---

#### Decision Model for Communication

This model helps practitioners choose communication patterns by evaluating requirements for *latency*, *reliability*, and *interoperability* between quantum and classical components. It includes patterns such as **Quantum Proxy**, **Broker-Client Separation**, and **Quantum API Gateway**, which enhance *modularity*, *scalability*, and *interoperability* while introducing trade-offs in *availability* and *performance*. Gateways determine suitable paths depending on whether secure communication, service abstraction, or hardware selection is prioritized.

<br>

<p align="center">
   <img src="https://github.com/user-attachments/assets/ce1663e1-1d5f-4398-821e-41246e8cf7d0" alt="Decision Model for Communication"  width="650" height="800">
</p>

---

#### Decision Model for Decomposition

The decomposition model structures quantum systems into manageable modules. It begins with **Quantum Microservices**, promoting *maintainability*, *scalability*, and *performance*, but with reduced *flexibility*. For layered-based decomposition, patterns like **Quantum Layered**, **Quantum Multi-Tier**, and **Recursive Containment** are selected based on system needs. These improve *extensibility*, *modularity*, and *portability*, but may impact *cost*, *reliability*, or *complexity*. Additionally, functionality-based decomposition uses **Single Responsibility** or **Decomposed by Business Capabilities** patterns to enhance *maintainability* and *performance*.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/abf6aca3-9bb2-4a58-b5ba-ec9340e37977" alt="Decision Model for Decomposition"  width="650" height="450">
</p>

---

#### Decision Model for Data Processing

This model guides the selection of data handling patterns through inclusive and exclusive gateways. When managing multi-stage data processing, the **Pipe and Filter** pattern enhances *flexibility* but may reduce *performance*. On-demand management leads to the **Consumer** pattern, while dynamic testing activates **Data-Driven Testing**. Advanced encoding needs activate patterns like **Quantum Data Encoding**, **Amplitude Encoding**, **Angle Encoding**, and **Basis Encoding**, each balancing trade-offs among *scalability*, *performance*, and *complexity*. For integration and conversion of quantum-classical data, **Quantum Mediator Wrapper** and **Measurement** patterns are used.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/477289f6-a289-4a35-8336-00433a5365f1" alt="Decision Model for Data Processing"  width="650" height="550">
</p>

---

#### Decision Model for Fault Tolerance

Focused on improving *reliability* and fault resilience, this model begins with inclusive gateways to assess tolerance and detection requirements. **Sparing**, **Comparison**, and **Voting** patterns are selected for redundancy and fault detection, offering strong *fault recovery* and *reliability* but with *performance* and *complexity* trade-offs. For correction, **Error Correction**, **Readout Error Mitigation**, and **Gate Error Mitigation** address specific fault sources. Additionally, **Decorator Design Pattern** and **Quantum Patterns of Behavior (qPoB)** offer high-level fault mitigation mechanisms, enhancing *adaptability* but increasing *system complexity*.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/16e0d7b8-76f9-4789-bb60-80f9143d2a42" alt="Decision Model for Fault Tolerance"  width="650" height="550">
</p>


---

#### Decision Model for Integration and Optimization

This model addresses the seamless integration of quantum components and optimization of operations. If integration is needed across quantum frameworks, the **Integration Pattern** is chosen. Optimization goals lead to selection among patterns like **Prototype Design**, **Quantum Broadcast**, **Decorator Design**, and **Quantum Transformer**, each affecting *extensibility*, *maintainability*, or *modularity*. Service-based integration activates **Quantum Service-Oriented Architecture**, **Quantum Service Registry**, **Bring Your Own Container (BYOC)**, and **Quantum Load Balancing**, depending on deployment needs, promoting *flexibility*, *discoverability*, and *resource optimization*.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/316c8c90-ec53-44b0-9842-9e4887ed3bc2" alt="Decision Model for Integration and Optimization"  width="650" height="500">
</p>

---

#### Decision Model for Algorithm Implementation

This model supports the design of quantum algorithms through modular and reusable patterns. The **Hybrid Module** pattern integrates classical and quantum logic, while the **Quantum-Classic Split** and **Classical-Quantum Interface** patterns allow separation of concerns and simplified integration. For reusable module design, **Quantum Module Pattern** and **Quantum Module Template** offer *flexibility* and *adaptability*. Optimizing execution involves selecting **Qubit Gate**, **Brickwork**, or **Template-Matching** patterns. Finally, for hardware portability and cross-platform compatibility, the **Quantum Circuit Translator** ensures *interoperability* across diverse quantum backends.

<br>
<p align="center">
   <img src="https://github.com/user-attachments/assets/3e17d951-b6b2-4e52-bade-407e94c5ce14" alt="Decision Model for Algorithm Implementation"  width="650" height="400">
</p>

---

### Stage 3: Evaluation of Decision Models
<p>
To evaluate the proposed decision models, we conducted semi-structured interviews with 16 practitioners using a standardized [interview questionnaire](https://docs.google.com/document/d/1lz0-mAz9rU2OQdewvDSbIYnGNEZQOm6c2t0XgT6iWnQ/edit?usp=sharing). The results of this evaluation are organized into two parts: (1) participant demographic and professional background, and (2) evaluation of the decision models with respect to familiarity, understandability, and correctness.
</p>


### Participant Demographics and Professional Background

<p>
To evaluate the decision models, we conducted semi-structured interviews with 16 practitioners from Asia, Africa, and Europe. Most participants had 6–10 years of experience in software development, and 2–10 years in quantum software development. Their roles ranged from researchers and developers to physicists and project managers, reflecting the interdisciplinary nature of the field. They were also involved in various quantum domains such as cryptography, AI/ML, optimization, simulation, and healthcare, often contributing to multiple domains simultaneously.
</p>
<p align="center">
   <img src="https://github.com/user-attachments/assets/8d4fbd12-b655-4f4e-a1e4-44bada1ac130" alt="Decision Models for Selecting Patterns and Strategies in Quantum Software Systems-Demography"  width="600" height="450">
</p>


### Practitioner Feedback on Decision Models

<p>
Practitioners generally reported high familiarity with the architectural patterns and strategies in the six proposed decision models. They found the models understandable, well-structured, and easy to apply in practice. All six models were considered sufficient for supporting architectural decisions in quantum software systems. Suggestions included adding more explicit trade-offs, clarifying relationships between patterns and quality attributes, and improving directional guidance. These inputs were incorporated into updated versions of the models.
</p>

<p align="center">
   <img src="https://github.com/user-attachments/assets/2d856397-afa1-4729-8413-f710c72de257" alt="Overview of practitioners’ responses for familiarity, understandability, and completeness of the decision models"  width="600" height="400">
</p>




