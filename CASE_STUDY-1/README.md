# Prompt Architecture Case Study #1
## Modular Prompting Case Study – Overview

If you want to help, PR or reach out on discord - https://discord.gg/Me6FK2sFVs
### Introduction
This study aims to address gaps in systematic benchmarking of prompting techniques, an open challenge for the field of prompt architecture. Specific goals are comparing performance across models and gathering optimization insights through standardized tests.  
**Independent Researcher. NO BUDGET. Educate the World.**

### Requirements
1. Test capabilities of GPT-3, GPT-4, Bard, Bing and Claude based on accessibility through free tiers and range of capacities.
2. Use accuracy, coherence, relevance, and efficiency metrics. Provide precise definitions and scales.
3. Specify statistical tests upfront and minimum significance level.
4. Document all prompt examples, model configurations, and experimental protocols for reproducibility.

### Research Questions

- **RQ1:** How do the accuracy levels of GPT-3, GPT-4, and Claude differ across the GSM8K arithmetic and Complex (CommaQA) reasoning tasks when using Zero-Shot Reasoning, Chain-of-Thought, and Decomposed Prompting techniques?

- **RQ2:** In the context of the GSM8K arithmetic tasks, which prompting technique results in the most logically consistent answers across GPT-3, GPT-4, and Claude?

- **RQ3:** For the Complex (CommaQA) reasoning tasks, which prompting technique leads to answers that most accurately address the posed questions for GPT-3, GPT-4, and Claude?

- **RQ4:** How do slight variations in input prompts (rephrasing, specificity changes, and ordering alterations) impact the consistency of responses from GPT-3, GPT-4, and Claude across both datasets?

- **RQ5:** What specific types of errors are most prevalent for each model across the GSM8K and CommaQA datasets? How might these errors impact the practical application of these models in real-world reasoning tasks?



### Framework
This comparative cumulative case study will evaluate three modular prompting techniques on established reasoning tasks across three large language models. The evolution of techniques will be summarized prior to the comparative assessment. Both quantitative metrics and qualitative analyses will be used to gather insights. These modular prompting techniques are reviewed in a literature review published by the researcher in peer reviewed journal [here](https://www.ijcaonline.org/archives/volume185/number34/ansara-2023-ijca-923133.pdf) 


### Objectives
- Benchmark performance of prompting techniques across models
- Gather comparative insights into optimization
- Establish baseline metrics as a reference
- Address gaps in systematic evaluations of prompting approaches

### Scope
The case study will focus on standardized tests of a select few prompting techniques on established reasoning datasets. Both quantitative metrics and qualitative human assessments will be utilized to gather comparative insights across models. The results will be interpreted in relation to predefined research goals and hypotheses. Limitations such as small sample sizes will be acknowledged.

### Models
GPT-3 was selected given its strong few-shot learning capabilities evidenced in prior work. GPT-4 provides a more recent contrast. Claude represents a similar GPT style AI and allows for extended comparisons.

### Techniques/Methods
- **Zero-Shot Reasoning:** hypothetically tests inherent reasoning skills with minimal prompting.
- **Chain-of-Thought:** utilizes step-by-step reasoning examples to guide models. This may improve multi-step inference but relies on prompt quality.
- **Decomposed Prompting:** aims to improve complex reasoning through modular subtask prompts. Effectiveness depends on decomposition.

### Reasoning Tasks
*This study will use the following Reasoning Tasks and associated Datasets*

| Reasoning Task                          | DataSet Name                  | Paper                                                                                     | GitHub                                                                                     |
|-------------------------------|------------------------------|------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
| Arithmetic                    | GSM8K                        | [Paper](https://arxiv.org/pdf/2110.14168v1.pdf)                                          | [Github](https://github.com/openai/grade-school-math)                                     |
| Complex Tasks            | CommaQA                   | [Paper](https://arxiv.org/abs/2110.08542)                                                | [Github](https://github.com/allenai/CommaQA)                                         |

See the Method_Guide for all the gooey details [here](CASE_STUDY-1/Method_Guide.md)




