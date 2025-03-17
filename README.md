# Awesome-Long2short-on-LRMs

Awesome-Long2short-on-LRMs is a collection of state-of-the-art, novel, exciting **long2short** methods on **large reasoning models**. It contains papers, codes, datasets, evaluations, and analyses.

**Content**
- [Prompt Guidance](#prompt-guidance)
- [Decoding Strategy](#decoding-strategy)
- [Latent Compression](#latent-compression)
- [Parameter Modification](#parameter-modification)
- [Others](#others)

## Prompt Guidance
> Prompt guidance generally includes budget guidance and template guidance.

| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.03 | **How Well do LLMs Compress Their Own Chain-of-Thought? A Token Complexity Approach** | arXiv | [link](https://arxiv.org/abs/2503.01141) | [link](https://github.com/Compressed-CoT/compressed-cot) |
| 2025.03 | **Sketch-of-Thought: Efficient LLM Reasoning with Adaptive Cognitive-Inspired Sketching** | arXiv | [link](https://arxiv.org/pdf/2503.05179v1) | [link](https://github.com/SimonAytes/SoT) |
| 2025.02 | **Meta-Reasoner: Dynamic Guidance for Optimized Inference-time Reasoning in Large Language Models** |   arXiv     | [link](https://arxiv.org/pdf/2502.19918) |        -      |
| 2025.02 | **Chain of Draft: Thinking Faster by Writing Less** |   arXiv     | [link](https://arxiv.org/pdf/2502.18600) |        [link](https://github.com/sileix/chain-of-draft)      |
| 2025.02 | **Stepwise Perplexity-Guided Refinement for Efficient Chain-of-Thought Reasoning in Large Language Models** |   arXiv     | [link](https://arxiv.org/abs/2502.13260) |        -      |
| 2024.12 | **Token-Budget-Aware LLM Reasoning** | arXiv | [link](https://arxiv.org/abs/2412.18547) | [link](https://github.com/GeniusHTX/TALE) |
| 2024.07 | **Concise Thoughts: Impact of Output Length on LLM Reasoning and Cost** | arXiv | [link](https://arxiv.org/abs/2407.19825) | - |
| 2023.05 | **Chain-of-Symbol Prompting Elicits Planning in Large Langauge Models** |   arXiv     | [link](https://arxiv.org/abs/2305.10276) |        [link](https://github.com/hanxuhu/chain-of-symbol-planning)    |

## Decoding Strategy

| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.02 | **When More is Less: Understanding Chain-of-Thought Length in LLMs** |   arXiv     | [link](https://arxiv.org/abs/2502.07266) |        -    |
| 2024.12 | **Efficiently Serving LLM Reasoning Programs with Certaindex** |   arXiv     | [link](https://arxiv.org/abs/2412.20993) |        [link](https://github.com/hao-ai-lab/Dynasor)    |



## Latent Compression
| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.02 | **LightThinker: Thinking Step-by-Step Compression** |   arXiv     | [link](https://arxiv.org/abs/2502.15589) |        [link](https://github.com/zjunlp/LightThinker)      |
| 2025.02 | **Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach** | arXiv | [link](https://arxiv.org/pdf/2502.05171) | [link](https://github.com/seal-rg/recurrent-pretraining) |
| 2025.02 | **Token Assorted: Mixing Latent and Text Tokens for Improved Language Model Reasoning** | arXiv | [link](https://arxiv.org/abs/2502.03275) | - |
| 2025.01 | **Efficient Reasoning with Hidden Thinking** | arXiv | [link](https://arxiv.org/abs/2501.19201) | - |
| 2024.12 | **Training Large Language Model to Reason in a Continuous Latent Space** | arXiv | [link](https://arxiv.org/pdf/2412.06769v2) | [link](https://github.com/facebookresearch/coconut) |
| 2024.12 | **Compressed Chain of Thought: Efficient Reasoning through Dense Representations** | arXiv | [link](https://arxiv.org/pdf/2412.13171) |    -   |
| 2024.05 | **From Explicit CoT to Implicit CoT: Learning to Internalize CoT Step by Step** | arXiv | [link](https://arxiv.org/pdf/2405.14838) | [link](https://github.com/da03/internalize_cot_step_by_step) |
| 2024.03 | **Quiet-STaR: Language Models Can Teach Themselves to Think Before Speaking** | arXiv | [link](https://arxiv.org/abs/2403.09629) | [link](https://github.com/ezelikman/quiet-star) |



## Parameter Modification
> Parameter modification generally includes SFT/RL, model merging, model distillation and so on.

| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.03 | **Optimizing Test-Time Compute via Meta Reinforcement Finetuning** |   arXiv     | [link](https://arxiv.org/pdf/2503.07572) |        [link](https://github.com/CMU-AIRe/MRT)    |
| 2025.03 | **DAST: Difficulty-Adaptive Slow-Thinking for Large Reasoning Models** |   arXiv     | [link](https://arxiv.org/abs/2503.04472) |        -    |
| 2025.03 | **L1: Controlling How Long A Reasoning Model Thinks With Reinforcement Learning** | arXiv | [link](https://www.arxiv.org/pdf/2503.04697) | [link](https://github.com/cmu-l3/l1) |
| 2025.03 | **InftyThink: Breaking the Length Limits of Long-Context Reasoning in Large Language Models** |   arXiv     | [link](https://arxiv.org/abs/2503.06692) |        -     |
| 2025.03 | **EAGLE-3: Scaling up Inference Acceleration of Large Language Models via Training-Time Test** | arXiv | [link](https://arxiv.org/pdf/2503.01840v1) | [link](https://github.com/SafeAILab/EAGLE) |
| 2025.02 | **Do NOT Think That Much for 2+3=? On the Overthinking of o1-Like LLMs** |   arXiv     | [link](https://arxiv.org/abs/2412.21187) |        -    |
| 2025.02 | **Self-Training Elicits Concise Reasoning in Large Language Models** |   arXiv     | [link](https://arxiv.org/abs/2502.20122) |        [link](https://github.com/TergelMunkhbat/concise-reasoning)    |
| 2025.02 | **TokenSkip: Controllable Chain-of-Thought Compression in LLMs** |   arXiv     | [link](https://arxiv.org/abs/2502.12067) |        [link](https://github.com/hemingkx/TokenSkip)     |
| 2025.02 | **s1: Simple test-time scaling** |   arXiv     | [link](https://arxiv.org/abs/2501.19393) |        [link](https://github.com/simplescaling/s1)     |
| 2025.02 | **CoT-Valve: Length-Compressible Chain-of-Thought Tuning** |   arXiv     | [link](https://arxiv.org/abs/2502.09601) |        [link](https://github.com/horseee/CoT-Valve)     |
| 2025.02 | **Training Language Models to Reason Efficiently** |   arXiv     | [link](https://arxiv.org/abs/2502.04463) |        [link](https://github.com/Zanette-Labs/efficient-reasoning)     |
| 2025.02 | **Claude 3.7 Sonnet and Claude Code** | Anthropic | [link](https://www.anthropic.com/news/claude-3-7-sonnet) | - |
| 2025.01 | **Kimi k1.5: Scaling Reinforcement Learning with LLMs** |   arXiv     | [link](https://arxiv.org/abs/2501.12599) |        -     |
| 2025.01 | **O1-Pruner: Length-Harmonizing Fine-Tuning for O1-Like Reasoning Pruning** |   arXiv     | [link](https://arxiv.org/abs/2501.12570) |        [link](https://github.com/StarDewXXX/O1-Pruner)     |
| 2024.12 | **C3oT: Generating Shorter Chain-of-Thought without Compromising Effectiveness** | arXiv | [link](https://arxiv.org/abs/2412.11664) | - |
| 2024.11 | **Can Language Models Learn to Skip Steps?** | arXiv | [link](https://arxiv.org/abs/2411.01855) | [link](https://github.com/tengxiaoliu/LM_skip) |
| 2023.10 | **Think before you speak: Training Language Models With Pause Tokens** |   arXiv     | [link](https://arxiv.org/abs/2310.02226v3) |        -     |

## Others
| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2024.12 | **Bag of Tricks for Inference-time Computation of LLM Reasoning** | arXiv | [link](https://arxiv.org/abs/2502.07191) | [link](https://github.com/usail-hkust/benchmark_inference_time_computation_LLM) |







## Contributors
<a href="https://github.com/Hongcheng-Gao" target="_blank"><img src="https://avatars.githubusercontent.com/u/96536860?v=4" alt="Hongcheng-Gao" width="72" height="72"/></a> 
<a href="https://github.com/xinlong-yang" target="_blank"><img src="https://avatars.githubusercontent.com/u/73691354?v=4" alt="xinlong-yang" width="72" height="72"/></a> 
<a href="https://github.com/yueliu1999" target="_blank"><img src="https://avatars.githubusercontent.com/u/41297969?s=64&v=4" alt="yueliu1999" width="72" height="72"/></a> 
<a href="https://github.com/ColorDavid" target="_blank"><img src="https://avatars.githubusercontent.com/u/57055043?v=4" alt="ColorDavid" width="72" height="72"/></a> 
<a href="https://github.com/junming-yang" target="_blank"><img src="https://avatars.githubusercontent.com/u/60545459?v=4" alt="junming-yang" width="72" height="72"/></a> 
<a href="https://github.com/yili-19" target="_blank"><img src="https://avatars.githubusercontent.com/u/61128160?v=4" alt="yili-19" width="72" height="72"/></a> 



























