### Zero Shot Reasoning 
**Paper:** Kojima, T., Gu, S.S., Reid, M., Matsuo, Y. and Iwasawa, Y. (2022). Large Language Models are Zero-Shot Reasoners. *arXiv:2205.11916 [cs]*. [online] Available at: <https://arxiv.org/abs/2205.11916>

#### Key Contributions
- Demonstrates LLMs have inherent zero-shot reasoning ability when prompted to "think step-by-step" across 12 diverse benchmark reasoning tasks.
- Proposes "Zero-shot Chain of Thought" (Zero-shot-CoT) prompting approach that significantly improves zero-shot LLM performance without any task-specific examples.
- Shows Zero-shot-CoT substantially outperforms standard zero-shot prompting and approaches/matches few-shot performance on tasks like MultiArith, GSM8K, and symbolic reasoning.
- Provides strong evidence that scaling model size leads to qualitative improvements in reasoning under Zero-shot-CoT prompting.
- Suggests latent multi-task reasoning skills encoded in LLMs that can be extracted via a simple, task-agnostic prompt.

#### Methodology
- Uses fixed prompt "Let's think step-by-step" before answer to elicit step-wise reasoning chain.
- Employs two-stage prompting process: First extract full reasoning chain, then extract final answer using tailored answer prompts.
- Tests on 12 diverse reasoning datasets: 6 arithmetic (MultiArith, GSM8K, etc), 2 commonsense (CommonsenseQA, StrategyQA), 2 symbolic (Last Letter, Coin Flip), and 2 logical (BIG-bench)
- Compares Zero-shot vs Zero-shot-CoT and Few-shot vs Few-shot-CoT on accuracy.
- Evaluates 17 LLMs ranging from 300M to 540B parameters, including GPT-3, InstructGPT, PaLM. 
- Analyzes 50 sample outputs per condition for reasoning quality and categorizes common error types.
- Tests prompt robustness using 15 variations of reasoning prompts.
- Evaluates model scaling effects from 300M to 540B parameters.
- Provides full prompts and answer cleansing details needed for reproducibility.

#### Reproducibility
- Greedy decoding used for most models, top-k sampling for PaLM.
- Fixed random seeds used for variance where applicable.
- Detailed prompt templates provided in Appendices A.5 and B.
- Complete list of models and datasets provided in Appendices A.2, A.3.  
- Answer cleansing methodology outlined in Appendix A.6.
- Analyzed reasoning chains included in Appendices B and C.
- Code to reproduce key experiments available on GitHub.

#### Significance
- Establishes strong zero-shot baseline for benchmarking reasoning tasks.
- Provides blueprint for discovering latent LLM capabilities via prompting.
- Demonstrates power of simple prompting to unlock complex cognitive skills.
- Motivates research into inherent multi-task abilities encoded in LLMs.
- Advances Prompt Architecture toward generalized, task-agnostic prompts.