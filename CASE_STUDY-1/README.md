# Prompt Architecture Case Study #1
## Modular Prompting Case Study – Overview

If you want to help, PR or reach out on discord - https://discord.gg/Me6FK2sFVs
### Introduction
This study aims to address gaps in systematic benchmarking of prompting techniques, an open challenge for the field of prompt architecture. Specific goals are comparing performance across models and gathering optimization insights through standardized tests.  
**Independent Researcher. NO BUDGET. Educate the World.**

### Requirements
1. Test capabilities of GPT-3, GPT-4, and Claude based on accessibility through free tiers and range of capacities.
2. Use accuracy, coherence, relevance, and efficiency metrics. Provide precise definitions and scales.
3. Specify statistical tests upfront and minimum significance level.
4. Document all prompt examples, model configurations, and experimental protocols for reproducibility.

### Research Questions
- **RQ1:** How do Zero-Shot Reasoning, Chain-of-Thought, and Decomposed Prompting techniques differ in accuracy across GSM8K arithmetic, Symbolic (Coin Flip), and Commonsense (CSQA) reasoning tasks?
- **RQ2:** How do the coherence and relevance outcomes of GPT-3, GPT-4, and Claude differ when applying the Zero-Shot Reasoning, Chain-of-Thought, and Decomposed Prompting techniques?
- **Additional Questions we’re going to try if we can…**
  - **RQ3:** How does the Chain-of-Thought prompting technique influence the multi-step reasoning capabilities of GPT-3, GPT-4, and Claude compared to standard prompting?
  - **RQ4:** Does the Decomposed Prompting technique enhance the performance of LLMs like GPT-3 and Claude in complex reasoning tasks compared to Chain-of-Thought prompting?
  - **RQ5:** To what extent does the Zero-Shot-CoT approach improve the zero-shot reasoning abilities of GPT-3 and GPT-4 across diverse tasks?

### Framework
This comparative cumulative case study will evaluate three modular prompting techniques on established reasoning tasks across three large language models. The evolution of techniques will be summarized prior to the comparative assessment. Both quantitative metrics and qualitative analyses will be used to gather insights.

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
| Implicit Reasoning            | StrategyQA                   | [Paper](https://arxiv.org/abs/2101.02235)                                                | [Github](https://github.com/eladsegal/strategyqa)                                         |
| Commonsense                   | CSQA                         | [Paper](https://arxiv.org/abs/1801.10314)                                                | [Github](https://github.com/amritasaha1812/CSQA_Code)                                     |

  
### Metrics for Evaluation

The following metrics have been identified for a comprehensive evaluation of the models on the specified tasks:

1. **Accuracy:** 
   - Defined as the ratio of correct responses to total responses.
   - Formula: `(Number of Correct Responses / Total Responses) * 100`

2. **Logical Consistency:** 
   - Evaluates the logical soundness of the model's responses. This metric is especially pertinent for tasks that demand logical reasoning, such as Arithmetic GSM8K.

3. **Depth of Reasoning:** 
   - Assesses the model's capability to provide detailed explanations or engage in multi-step reasoning. This is particularly relevant for tasks like StrategyQA that require deeper cognitive processing.

4. **Error Categorization:** 
   - Involves a systematic breakdown of the errors made by the model into specific categories, such as arithmetic errors or reasoning errors. This categorization aids in understanding the specific areas where the model might require improvement.

5. **Robustness to Input Variation:** 
   - Measures the consistency in the model's responses when presented with prompts that are slightly varied or rephrased. This metric ensures that the model's performance is not overly sensitive to specific phrasings.

These metrics aim to provide a holistic view of the model's performance across various dimensions, ensuring a thorough and unbiased evaluation.


### Data Collection
GUI Chats & model APIs with rate limits

### Analysis
Quantitative metrics such as accuracy will be supplemented by qualitative human judgements of coherence and relevance. Comparisons will highlight differences in optimization between techniques and models. Be wary of biases and consider crowd-sourcing some evaluations.

### Limitations
The small sample of models and techniques limits generalizability. Lack of real-world evaluation makes it unclear how findings would translate to applied settings. While findings may not fully generalize, this initial comparative study will provide the foundation for future work expanding the models, techniques, and real-world evaluations.

### Conclusion
The conclusion will summarize key takeaways from the comparative assessments, framing actionable insights for prompt architecture.



