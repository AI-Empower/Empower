# Datasets & Reasoning Tasks
## Introduction

Welcome to our repository of major datasets used in Prompt Architecture Testing. There are thousands of datasets in the world, we chose these because we see other major researchers using them, and we want to encourage standing on the shoulders of the giants who came before us. These datasets are invaluable tools for researchers aiming to solve complex problems in areas such as math word problems, commonsense reasoning, symbolic reasoning, and more. 


Whether you're a seasoned researcher or a beginner in the field, this list of datasets offer a comprehensive range of data to test, validate, and implement your prompts and prompt architecture concepts.


## How to Test Different Types of Reasoning Tasks

Testing different types of reasoning tasks requires a well-thought-out approach, as each type of reasoning has its own unique challenges and requirements. I'll try to include some basic guidelines under each category. 

### Independant researchers
If you're looking to test Prompt Architecture comprehensively but still stay within reasonable goals, consider dropping the the 4 more complex categories - Multi-hop QA, Decomposition, Robot Planning & Sports Plausibility, then picking one from each of the 5 remaining categories. 

## Math Word Problems
- GSM8K Dataset
  - [Paper](https://arxiv.org/pdf/2110.14168v1.pdf) and [Github](https://github.com/openai/grade-school-math)
- SVAMP Dataset
  - [Paper](https://arxiv.org/abs/2103.07191) and [Github](https://github.com/arkilpatel/SVAMP)
- ASDiv
  - [Paper](https://www.aclweb.org/anthology/2020.acl-main.92.pdf) and [Github](https://github.com/chaochun/nlu-asdiv-dataset).
- MAWPS
  - [Paper](https://www.aclweb.org/anthology/N16-1136.pdf) and [Github](https://github.com/sroy9/mawps).


For math word problems, it's essential to test not only the accuracy of the solution but also the model's ability to understand the problem context. You can use metrics like F1-score and accuracy to evaluate performance.

## Arithmetic Reasoning
- MultiArith
- AddSub
- SingleEq

Arithmetic reasoning tasks can be evaluated based on the model's ability to perform calculations accurately and efficiently. Speed and accuracy are key metrics here.

## Commonsense Reasoning
- CSQA [Paper](https://arxiv.org/abs/1801.10314) and [Github](https://github.com/amritasaha1812/CSQA_Code)
- StrategyQA [Paper](https://arxiv.org/abs/2101.02235) and [Github](https://github.com/eladsegal/strategyqa)

In commonsense reasoning, the focus should be on the model's ability to make logical deductions that are not explicitly stated. Techniques like ablation studies can be useful here.

## Symbolic Reasoning
- Last Letter Concatenation
- Coin Flip

Symbolic reasoning often involves manipulating symbols according to certain rules. Here, you may want to look at how well the model generalizes across different types of symbolic tasks.

## Multi-hop QA
- HotpotQA
- CommaQA
- MuSiQue
- 2WikiMultihopQA

In multi-hop QA tasks, the model needs to gather information from multiple sources to answer a question. Evaluation could involve measuring the model's ability to correctly identify and utilize these sources.

## Decomposition
- List Reversal
- kth Letter Concatenation

For decomposition tasks, the key is to evaluate how well the model can break down a complex problem into simpler sub-problems. Metrics like precision and recall can be useful.

## Robot Planning & Sports Plausibility
- SayCan
- Sports Understanding

In these specialized tasks, domain-specific evaluation metrics are often required to accurately assess performance.

## Other Logical Reasoning
- Date Understanding
- Tracking Shuffled Objects

<<<<<<< 
For other types of logical reasoning, it's important to consider the model's ability to understand and apply rules or principles that are not explicitly stated. Custom evaluation metrics may be needed.
>>>>>>>


## Help us attrib
This article needs work. Feel free to help :)