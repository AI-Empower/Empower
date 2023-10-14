# Decomposed Prompting: A Modular Approach for Solving Complex Tasks
Khot, T., Trivedi, H., Finlayson, M., Fu, Y., Richardson, K., Clark, P. and Sabharwal, A. (2023). Decomposed Prompting: A Modular Approach for Solving Complex Tasks. [online] arXiv.org. doi:https://doi.org/10.48550/arXiv.2210.02406 
## Summary

This paper introduces Decomposed Prompting (DECOMP), which decomposes complex reasoning tasks into specialized sub-tasks handled by separate prompt-based modules. It enables recursive decomposition and integration of symbolic functions. DECOMP substantially improves over chain-of-thought prompting, demonstrating the power of modular, targeted prompting.

## Prompts

DECOMP operates by generating a decomposition program using a "decomposer" prompt. Sub-tasks are delegated to specialized "handler" prompts optimized for those skills. Handlers can recursively decompose or integrate external functions.

## Models 

DECOMP was evaluated on various sized LLMs including GPT-3, PaLM, and Flan-T5 without task-specific fine-tuning.

## Experimental Protocols

Tasks include symbolic reasoning, QA, and open-domain QA. DECOMP variants are compared to baselines like chain-of-thought prompting. Prompt robustness is analyzed across variations.

## Methodology

DECOMP's key innovation is the decomposer generating programs calling specialized sub-task handlers. This allows:

- Targeted optimization of each prompt 
- Recursive decomposition
- Integration of symbolic functions  
- Modular upgrades to components

## Key Contributions

DECOMP provides:

- A systematic, modular framework for complex reasoning
- Targeted elicitation of skills through decomposition  
- A new SotA for few-shot prompting

## Main Arguments

The authors argue decomposition enables prompting techniques to handle more complex tasks than possible with monolithic approaches. Specialized prompts for each sub-task are more effective.

## Limitations

- Limited analysis of cross-task generalization
- Focused on exact match accuracy
- Requires manual creation of decomposition prompts

## Impact

DECOMP provides a compelling paradigm for few-shot reasoning through targeted decomposition. The modular framework enables complex skills with minimal training.

## Next Steps

Future work could:

- Automate decomposer prompt generation
- Apply to open-ended generation tasks
- Analyze factual accuracy and logical consistency
- Explore cross-task and cross-domain decomposition