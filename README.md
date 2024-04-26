<p align="center">
    <img src="https://github.com/shamimaaktar1/ADDMQSA/assets/75358854/4cf274b1-0c26-4867-9475-c1eb5a3973a2" alt="chatGPT logo" width="180" height="250">
</p>

<h2 align="center">Decision Models for Selecting Patterns and Strategies in Quantum Software Systems</h3>

<p align="left">
  This is the replication package for the paper: "Decision Models for Selecting Patterns and Strategies in Quantum Software Systems", including the dataset, figures,  scripts, and so on (see the description below).
  <br>

  
## File Organization

1. `Dataset.xlsx` contains the information about i) selected GitHub projects, ii) selected Stack Exchange sites, iii) selected GitHub issues, iv) Selected Stack Exchange posts, v) raw data of GitHub issues, vi) raw data of stack exchange posts, vii) pattern and strategy impact.
2. `Decision Models` folder contains the high-quality figures of the four decision models, namely, the decision model for I) structural abstraction, ii) communications, iii) integration and optimization, iv) data processing.


## Experiment Replication Steps

This research paper is divided into three main phases.

- [Phase 1: Research Design](#research-design)
  - [Identifying Quantum Patterns and Strategies](#identifying-quantum-patterns-and-strategies)
  - [Modeling Decision Models](#modeling-decision-models)
  - [Evaluating Decision Models](#evaluating-decision-models)
  
- [Phase 2: Decision Models](#enabling-collaborative-architecting)
  - [Decision Model for Structural Abstraction](#decision-model-for-structural-abstraction)
  - [Decision Model for Communications](#decision-model-for-communications)
  - [Decision Model for Integration and Optimization](#decision-model-for-integration-and-optimization)
  - [Decision Model for Data Processing](#decision-model-for-data-processing)
- [Phase 3: Evaluation of Decision Models](#evaluation-of-decision-models)


### Phase 1: Research Design

<p>
These decision models were explicitly crafted for four critical areas of quantum software design: structural abstraction, communication, integration and optimization, and data processing. These areas were chosen because they are fundamental to addressing critical design, implementation, integration, and data management challenges.
</p>
The research method is described below and represented in the picture below:
<br>
<br>

<p align="center">
   <img src="https://github.com/shamimaaktar1/ADDMQSA/assets/75358854/bc868529-2ec2-43c0-9a41-362010e9aa7c" alt="Research Process"  width="650" height="600">
</p>



#### Identifying Quantum Patterns and Strategies

<p>
The required patterns, strategies, quality attributes, and impact of patterns on quality attributes for creating decision models are collected data from the two sources (e.g., GitHub1 and Stack Exchange sites 2) inspired by the guidelines for selecting empirical methods for software engineering research. The following are used to extract the relevant issues and posts from both GitHub and Stack Exchange sites.
</p>


#### Modeling Decision Models

<p>
The decision flow is represented using the Inclusive, Exclusive, and Parallel gateways from the Business Process Model and Notation (BPMN). Each area of quantum software architecture design is depicted using a grey box. A circle marks the commencement of a decision process. Inclusive gateways initiate multiple outgoing paths in a decision process, while Exclusive gateways activate a single outgoing path. Conversely, Parallel gateways facilitate several concurrent outgoing paths in the decision process. Rounded rectangles denote the patterns and strategies associated with a quantum software architecture design area. A bidirectional arrow indicates a “complements” relationship between two patterns or strategies. An octagon and a dashed arrow symbolize constraints for each pattern or strategy. The positive and negative influences of each pattern or strategy on the quality attributes are signified by plus (+) and minus (-) signs, respectively. 
</p>
<br>
<br>

<p align="center">
   <img src="https://github.com/shamimaaktar1/ADDMQSA/assets/75358854/8c52844e-dc48-46e9-af0b-c31c0d36e40f" alt="Model and Notation (BPMN)"  width="600" height="300">
</p>


#### Evaluating Decision Models

In our study, we conducted a survey of quantum software practitioners and aimed to refine and evaluate our decision models. We conducted a descriptive survey following the guidelines proposed by Kitchenham and Pfleeger. Our survey questionnaire was conducted using Google Forms.


### Phase 2: Decision Models

<p>
We proposed a set of decision models for selecting patterns and strategies in four areas of quantum software systems design: structural abstraction, communication, integration and optimization, and data processing. These decision models are proposed based on the knowledge collected from analyzing quantum software development discussions in GitHub issues and Stack Exchange posts. These models will help practitioners choose suitable patterns and strategies to address various design challenges in quantum software systems.
</p>
  
#### Decision Model for Structural Abstraction

<p>
The decision model for structural abstraction in quantum software system design is a comprehensive framework that guides practitioners in selecting the most appropriate architecture pattern
based on the impact for structural abstraction. Each pattern within the model serves a specific purpose and is evaluated based on its positive and negative impacts on these attributes.
</p>

  
#### Decision Model for Communications

<p>
The decision model for quantum communication aids practitioners in choosing the right communication pattern for quantum software systems by evaluating the impact of quality attributes. This model is vital for enhancing the interaction between quantum components to ensure eﬀiciency, reliability, and scalability. 
</p>

#### Decision Model for Integration and Optimization

<p>
The decision model for quantum integration and optimization aims to streamline the development and enhancement of quantum software systems by guiding the selection of appropriate architectural patterns based on the impact of quality attributes. This model helps practitioners integrate various programming techniques and optimize quantum operations, considering eﬀiciency, extensibility, and testability
</p>

#### Decision Model for Data Processing

<p>
The decision model for quantum data processing is crafted to simplify the handling, processing, and testing of quantum data within quantum software systems. It emphasizes Performance, Compatibility, Extensibility, and Flexibility in quantum computations.
</p>


### Phase 3: Evaluation of Decision Models

<p>
  To evaluate the decision models, we conducted a survey of the response 24 practitioners.
</p>









