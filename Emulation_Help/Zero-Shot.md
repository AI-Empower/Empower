# Large Language Models are Zero-Shot Reasoners
Kojima, T., Gu, S.S., Reid, M., Matsuo, Y. and Iwasawa, Y. (2022). Large Language Models are Zero-Shot Reasoners. arXiv:2205.11916 [cs]. [online] Available at: https://arxiv.org/abs/2205.11916 
## Summary 

This paper shows large language models like GPT-3 and PaLM exhibit strong inherent zero-shot reasoning abilities on diverse reasoning tasks when prompted with a simple template like "Let's think step-by-step." The approach, called Zero-shot Chain of Thought (Zero-shot-CoT), significantly improves performance without requiring any task-specific examples or training.

## Prompts

The main prompt tested is "Let's think step-by-step." The authors also evaluate the robustness across 15 variations of reasoning prompts.

## Models

A range of models from 300M to 540B parameters are tested, including GPT-3, InstructGPT, PaLM, GPT-2, GPT-Neo, and T0.

## Experimental Protocols

Models are prompted with Zero-shot-CoT and evaluated on 12 reasoning tasks using accuracy. Greedy decoding is primarily used. 50 samples per condition are analyzed. Prompt robustness is tested.

## Methodology

Zero-shot-CoT uses a two-stage prompting approach. First, the full reasoning chain is elicited, then the final answer is extracted. The single prompt is applied across diverse reasoning skills without per-task tuning.

## Key Contributions

- Demonstrates strong inherent zero-shot reasoning skills in LLMs extractable via prompting
- Proposes Zero-shot-CoT as a simple, task-agnostic approach to elicit complex multi-step reasoning 
- Provides new zero-shot baseline for benchmarking reasoning

## Main Arguments

Key arguments:

- LLMs exhibit untapped zero-shot reasoning potential accessible through prompting
- General, multi-task prompts can unlock complex cognitive skills 
- Scaling model size leads to better zero-shot reasoning performance

## Limitations

- Limited analysis of prompt sensitivity and comparisons to other techniques
- No guarantees on logical accuracy of generated reasoning chains
- Lack of full training data details for proprietary models 

## Impact

Establishes prompting as a powerful technique for eliciting complex skills from LLMs without training. Findings motivate investigating inherent multi-task capabilities encoded in models.

## Next Steps for Prompt Architecture  

Future directions:

- Automate prompt creation for Zero-shot-CoT
- Improve logical accuracy of generated reasoning
- Discover other latent multi-task capabilities via prompts  
- Compare Zero-shot-CoT to other prompting approaches
- Examine societal impacts