# Decomposed Prompting

## Key Contributions

- Introduces Decomposed Prompting (DECOMP) which decomposes complex tasks into separate specialized prompts for each sub-task.

- Enables hierarchical and recursive decomposition of difficult sub-tasks.

- Incorporates symbolic functions and APIs as modular components.

- Improves over chain-of-thought prompting by 14-17 points on math QA datasets.

## Methodology

- Uses a "decomposer" prompt to generate a program calling specialized sub-task prompts.

- Sub-tasks can recurse into simpler sub-tasks.

- Evaluated on symbolic reasoning, long-context QA, and open-domain QA.

- Tested recursive decomposition on list reversal.

- Integrated Elasticsearch retrieval for open-domain QA.

## Results

- DECOMP substantially outperforms chain-of-thought on all datasets.

- Specialized sub-task prompts are more effective than standard prompts. 

- Recursive decomposition enables length generalization.

- Retrieval integration improves open-domain QA by 15+ points.

## Significance 

- Establishes specialized sub-task prompts as a powerful technique.

- Provides a systematic, modular framework for complex reasoning.

- Uncovers latent skills in LLMs through targeted decomposition.

- Opens up new directions for modular and composable prompting.