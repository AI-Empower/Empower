

# Chain-of-Thought Prompting Elicits Reasoning in Large Language Models

Wei et al. (2023) introduce chain-of-thought prompting, a technique for eliciting complex multi-step reasoning from large language models (LMs) without task-specific training. 

## Prompts

The prompts demonstrate "chain of thought" reasoning by providing input-output pairs that decompose reasoning processes into multiple natural language steps. For example, arithmetic reasoning prompts break down multi-step word problems through equations and explanations. Commonsense reasoning prompts show inference chains. The full prompts cover diverse reasoning skills including arithmetic, algebra, commonsense, symbolic manipulation, and planning.

## Models

Experiments use four state-of-the-art LMs: LaMDA, GPT-3, PaLM, and Codex. The authors evaluate a range of model sizes from 350M to 540B parameters, without any task-specific finetuning.

## Experiments

The authors rigorously test chain-of-thought prompting on diverse reasoning tasks spanning arithmetic, commonsense, and symbolic domains. Accuracy is evaluated on 10 datasets after prompting models with just 8 examples. Ablations analyze the impact of different prompt variations. TPU chips are leveraged to enable experiments on large LMs.

## Methodology

This paper introduces an influential technique for eliciting complex multi-step reasoning from LMs. The key innovation is using prompts to provide demonstrations of step-by-step inference chains. This guides LMs to decompose problems and reason through them.

## Key Contributions 

This work makes two important contributions. First, it shows chain-of-thought prompting substantially improves reasoning over standard prompting across diverse skills. Second, it highlights the latent reasoning potential hidden within large LMs that can be unlocked with simple prompting approaches.

## Main Arguments

The authors make a compelling case that standard few-shot prompting struggles on complex reasoning tasks. They argue providing chain-of-thought reasoning demonstrations in prompts enables large LMs to decompose and solve such problems. This prompting approach elicits strong reasoning skills without any task-specific training.

## Limitations

While an important first step, there are several limitations. First, the work does not thoroughly analyze sensitivity to prompt variations. Second, it does not compare chain-of-thought prompting against other related prompting techniques. Finally, generated chains of thought do not guarantee logical reasoning. Improving factual generations remains an open problem.

## Impact 

This work introduces an influential technique for eliciting reasoning from LMs via prompts. Chain-of-thought prompting exemplifies guiding LMs through step-by-step inference. The approach underscores the latent capabilities within large LMs extractable with simple prompting.