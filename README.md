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

#### Decision Model for Communication

<p>
The decision model for quantum communication aids practitioners in choosing the right communication pattern for quantum software systems by evaluating their impact on key quality attributes. It enhances interactions between quantum and classical components to ensure <em>efficiency, reliability, and scalability</em> in distributed or hybrid quantum systems.
</p>

#### Decision Model for Decomposition

<p>
This model assists in decomposing complex quantum systems into smaller, modular components. It guides the selection of architectural strategies that improve <em>modularity, maintainability, scalability</em>, and <em>testability</em>. Such decomposition is critical in enabling manageable development and testing workflows in hybrid quantum-classical environments.
</p>

#### Decision Model for Data Processing

<p>
The data processing model supports architectural decisions involving the collection, transformation, and handling of quantum data. It highlights trade-offs across <em>performance, flexibility, extensibility</em>, and <em>compatibility</em>, particularly in scenarios where quantum and classical computations must interoperate efficiently.
</p>

#### Decision Model for Fault Tolerance

<p>
This model helps in selecting fault-tolerant architectural patterns designed to mitigate the inherent instability of quantum operations. It focuses on <em>reliability, robustness, performance</em>, and <em>complexity</em>, addressing the challenges of noise, decoherence, and error propagation in quantum circuits.
</p>

#### Decision Model for Integration and Optimization

<p>
The integration and optimization model facilitates decisions regarding the seamless combination of quantum and classical components and the optimization of quantum workflows. It supports trade-offs in <em>efficiency, extensibility, testability</em>, and <em>energy-performance</em>, enabling improved system performance in hybrid execution environments.
</p>

#### Decision Model for Algorithm Implementation

<p>
This model provides guidance for implementing quantum algorithms by considering algorithmic complexity, hardware limitations, and resource availability. It balances <em>correctness, performance, portability</em>, and <em>scalability</em>, helping practitioners make informed design choices aligned with both functional requirements and quality goals.
</p>


### Phase 3: Evaluation of Decision Models

<p>
  To evaluate the decision models, we conducted a survey of the responses 24 practitioners.
</p>









