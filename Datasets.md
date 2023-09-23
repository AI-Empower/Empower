# Major Datasets Used by Researchers
# Introduction

Welcome to our repository of major datasets used in Prompt Architecture Testing. These datasets are invaluable tools for researchers aiming to solve complex problems in areas such as math word problems, commonsense reasoning, symbolic reasoning, and more. Whether you're a seasoned researcher or a beginner in the field, these datasets offer a comprehensive range of data to test, validate, and implement your algorithms and models.

## How to Test Different Types of Reasoning Tasks

Testing different types of reasoning tasks requires a well-thought-out approach, as each type of reasoning has its own unique challenges and requirements. Below are some general guidelines:

### Math Word Problems
For math word problems, it's essential to test not only the accuracy of the solution but also the model's ability to understand the problem context. You can use metrics like F1-score and accuracy to evaluate performance.

### Commonsense Reasoning
In commonsense reasoning, the focus should be on the model's ability to make logical deductions that are not explicitly stated. Techniques like ablation studies can be useful here.

### Symbolic Reasoning
Symbolic reasoning often involves manipulating symbols according to certain rules. Here, you may want to look at how well the model generalizes across different types of symbolic tasks.

### Decomposition
For decomposition tasks, the key is to evaluate how well the model can break down a complex problem into simpler sub-problems. Metrics like precision and recall can be useful.

### Multi-hop QA
In multi-hop QA tasks, the model needs to gather information from multiple sources to answer a question. Evaluation could involve measuring the model's ability to correctly identify and utilize these sources.

### Arithmetic Reasoning
Arithmetic reasoning tasks can be evaluated based on the model's ability to perform calculations accurately and efficiently. Speed and accuracy are key metrics here.

### Other Logical Reasoning
For other types of logical reasoning, it's important to consider the model's ability to understand and apply rules or principles that are not explicitly stated. Custom evaluation metrics may be needed.

### Robot Planning and Sports Plausibility
In these specialized tasks, domain-specific evaluation metrics are often required to accurately assess performance.

By following these guidelines, you can ensure a comprehensive evaluation of your model across various reasoning tasks.

## Math Word Problems
- GSM8K
- SVAMP
- ASDiv
- AQuA
- MAWPS

## Commonsense Reasoning
- CSQA
- StrategyQA

## Symbolic Reasoning
- Last Letter Concatenation
- Coin Flip

## Decomposition
- List Reversal
- kth Letter Concatenation

## Multi-hop QA
- HotpotQA
- CommaQA
- MuSiQue
- 2WikiMultihopQA

## Arithmetic Reasoning
- MultiArith
- AddSub
- SingleEq

## Other Logical Reasoning
- Date Understanding
- Tracking Shuffled Objects

## Robot Planning
- SayCan

## Sports Plausibility
- Sports Understanding
