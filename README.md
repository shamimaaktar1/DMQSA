<p align="center">
    <img src="https://github.com/shamimaaktar1/ADDMQSA/assets/75358854/4cf274b1-0c26-4867-9475-c1eb5a3973a2" alt="chatGPT logo" width="180" height="250">
</p>

<h2 align="center">Decision Models for Selecting Patterns and Strategies in Quantum Software Systems</h3>

<p align="left">
  This is the replication package for the paper: "Decision Models for Selecting Patterns and Strategies in Quantum Software Systems", including the dataset, figures,  scripts, and so on (see the description below).
  <br>

  
## File Organization

1. `Dataset.xlsx` contains the information about i) selected GitHub projects, ii) selected Stack Exchange sites, iii) selected GitHub issues, iv) Selected Stack Exchange posts, v) raw data of GitHub issues, vi) raw data of stack exchange posts, vii) pattern and strategy impact.
2. `Decision Models` folder contains the high-quality figures of the four decision models, namely, the decision model for i) Communication, ii) Decomposition, iii) Data
Processing, iv) Fault Tolerance, v) Integration and Optimization, and vi) Algorithm Implementation.


## Experiment Replication Steps

This research paper is divided into three main phases.

- [Phase 1: Research Design](#research-design)
  - [Identifying Quantum Patterns and Strategies](#identifying-quantum-patterns-and-strategies)
  - [Modeling Decision Models](#modeling-decision-models)
  - [Evaluating Decision Models](#evaluating-decision-models)

- [Phase 2: Decision Models](#decision-models)
  - [Decision Model for Communication](#decision-model-for-communication)
  - [Decision Model for Decomposition](#decision-model-for-decomposition)
  - [Decision Model for Data Processing](#decision-model-for-data-processing)
  - [Decision Model for Fault Tolerance](#decision-model-for-fault-tolerance)
  - [Decision Model for Integration and Optimization](#decision-model-for-integration-and-optimization)
  - [Decision Model for Algorithm Implementation](#decision-model-for-algorithm-implementation)

- [Phase 3: Evaluation of Decision Models](#evaluation-of-decision-models)



### Phase 1: Research Design

<p>
The decision models were explicitly crafted for four critical areas of quantum software design: structural abstraction, communication, integration and optimization, and data processing. These areas were chosen because they are fundamental to addressing critical design, implementation, integration, and data management challenges.
</p>
The research method is described below and represented in the picture below:
<br>
<br>

<p align="center">
   <img src="https://github.com/shamimaaktar1/ADDMQSA/assets/75358854/bc868529-2ec2-43c0-9a41-362010e9aa7c" alt="Research Process"  width="650" height="600">
</p>



#### Identifying Quantum Patterns and Strategies

<p>
The required patterns, strategies, quality attributes, and impact of patterns on quality attributes for creating decision models are collected data from the two sources (e.g., GitHub and Stack Exchange sites) inspired by the guidelines for selecting empirical methods for software engineering research. The following are used to extract the relevant issues and posts from both GitHub and Stack Exchange sites.
</p>


#### Modeling Decision Models

<p>
The decision flow is represented using the Inclusive, Exclusive, and Parallel gateways from the Business Process Model and Notation (BPMN). Each area of quantum software architecture design is depicted using a grey box. A circle marks the commencement of a decision process. Inclusive gateways initiate multiple outgoing paths in a decision process, while Exclusive gateways activate a single outgoing path. Conversely, Parallel gateways facilitate several concurrent outgoing paths in the decision process. Rounded rectangles denote the patterns and strategies associated with a quantum software architecture design area. A bidirectional arrow indicates a “complements” relationship between two patterns or strategies. An octagon and a dashed arrow symbolize constraints for each pattern or strategy. The positive and negative influences of each pattern or strategy on the quality attributes are signified by plus (+) and minus (-) signs, respectively. 
</p>
<br>
<br>

<p align="center">
   <img src="https://github.com/shamimaaktar1/ADDMQSA/assets/75358854/8c52844e-dc48-46e9-af0b-c31c0d36e40f" alt="Model and Notation (BPMN)"  width="600" height="280">
</p>


#### Evaluating Decision Models

In our study, we conducted a survey of quantum software practitioners and aimed to refine and evaluate our decision models. We conducted a descriptive survey following the guidelines proposed by Kitchenham and Pfleeger. Our survey questionnaire was conducted using Google Forms.


### Phase 2: Decision Models

<p>
We proposed a set of decision models for selecting patterns and strategies in six critical areas of quantum software system design: <strong>Communication</strong>, <strong>Decomposition</strong>, <strong>Data Processing</strong>, <strong>Fault Tolerance</strong>, <strong>Integration and Optimization</strong>, and <strong>Algorithm Implementation</strong>. These models are developed based on insights gathered from analyzing real-world development discussions in GitHub issues and Stack Exchange posts. They aim to guide practitioners in addressing design challenges by providing structured pathways to select suitable architectural patterns and strategies while balancing relevant quality trade-offs.
</p>

### Phase 2: Decision Models

We present six decision models that guide practitioners in selecting architectural patterns and strategies across key design areas in quantum software systems. These models were derived from empirical analysis of practitioner discussions on GitHub and Stack Exchange and are structured using BPMN decision flows. Each model maps system conditions to patterns based on their influence on *quality attributes*.

---

#### Decision Model for Communication

This model helps practitioners choose communication patterns by evaluating requirements for *latency*, *reliability*, and *interoperability* between quantum and classical components. It includes patterns such as **Quantum Proxy**, **Broker-Client Separation**, and **Quantum API Gateway**, which enhance *modularity*, *scalability*, and *interoperability* while introducing trade-offs in *availability* and *performance*. Gateways determine suitable paths depending on whether secure communication, abstraction of services, or hardware selection is prioritized.

---

#### Decision Model for Decomposition

The decomposition model structures quantum systems into manageable modules. It begins with **Quantum Microservices**, promoting *maintainability*, *scalability*, and *performance*, but with reduced *flexibility*. For layered-based decomposition, patterns like **Quantum Layered**, **Quantum Multi-Tier**, and **Recursive Containment** are selected based on system needs. These improve *extensibility*, *modularity*, and *portability*, but may impact *cost*, *reliability*, or *complexity*. Additionally, functionality-based decomposition uses **Single Responsibility** or **Decomposed by Business Capabilities** patterns to enhance *maintainability* and *performance*.

---

#### Decision Model for Data Processing

This model guides the selection of data handling patterns through inclusive and exclusive gateways. When managing multi-stage data processing, the **Pipe and Filter** pattern enhances *flexibility* but may reduce *performance*. On-demand management leads to the **Consumer** pattern, while dynamic testing activates **Data-Driven Testing**. Advanced encoding needs activate patterns like **Quantum Data Encoding**, **Amplitude Encoding**, **Angle Encoding**, and **Basis Encoding**, each balancing trade-offs among *scalability*, *performance*, and *complexity*. For integration and conversion of quantum-classical data, **Quantum Mediator Wrapper** and **Measurement** patterns are used.

---

#### Decision Model for Fault Tolerance

Focused on improving *reliability* and fault resilience, this model begins with inclusive gateways to assess tolerance and detection requirements. **Sparing**, **Comparison**, and **Voting** patterns are selected for redundancy and fault detection, offering strong *fault recovery* and *reliability* but with *performance* and *complexity* trade-offs. For correction, **Error Correction**, **Readout Error Mitigation**, and **Gate Error Mitigation** address specific fault sources. Additionally, **Decorator Design Pattern** and **Quantum Patterns of Behavior (qPoB)** offer high-level fault mitigation mechanisms, enhancing *adaptability* but increasing *system complexity*.

---

#### Decision Model for Integration and Optimization

This model addresses the seamless integration of quantum components and optimization of operations. If integration is needed across quantum frameworks, the **Integration Pattern** is chosen. Optimization goals lead to selection among patterns like **Prototype Design**, **Quantum Broadcast**, **Decorator Design**, and **Quantum Transformer**, each affecting *extensibility*, *maintainability*, or *modularity*. Service-based integration activates **Quantum Service-Oriented Architecture**, **Quantum Service Registry**, **Bring Your Own Container (BYOC)**, and **Quantum Load Balancing**, depending on deployment needs, promoting *flexibility*, *discoverability*, and *resource optimization*.

---

#### Decision Model for Algorithm Implementation

This model supports the design of quantum algorithms through modular and reusable patterns. The **Hybrid Module** pattern integrates classical and quantum logic, while the **Quantum-Classic Split** and **Classical-Quantum Interface** patterns allow separation of concerns and simplified integration. For reusable module design, **Quantum Module Pattern** and **Quantum Module Template** offer *flexibility* and *adaptability*. Optimizing execution involves selecting **Qubit Gate**, **Brickwork**, or **Template-Matching** patterns. Finally, for hardware portability and cross-platform compatibility, the **Quantum Circuit Translator** ensures *interoperability* across diverse quantum backends.









