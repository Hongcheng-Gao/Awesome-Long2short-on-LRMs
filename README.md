# Awesome-Long2short-on-LRMs

Awesome-Long2short-on-LRMs is a collection of state-of-the-art, novel, exciting **long2short** methods on **large reasoning models**. It contains papers, codes, datasets, evaluations, and analyses.

**Content**
**Content**
- [Length-Aware Guidance](#length-aware-guidance)
  - [Prompt Guidance](#prompt-guidance)
    - [Active Prompt Guidance](#active-prompt-guidance)
    - [Passive Prompt Guidance](#passive-prompt-guidance)
  - [Reward Guidance](#reward-guidance)
- [Length-Agnostic Optimization](#length-agnostic-optimization)
  - [Latent Space Compression](#latent-space-compression)
  - [Routing Strategy](#routing-strategy)
    - [Template Routing](#template-routing)
    - [Solution Routing](#solution-routing)
  - [Computation Routing](#computation-routing)
  - [Model Distillation](#model-distillation)
    - [Model Distillation for Preference Learning](#model-distillation-for-preference-learning)
    - [Model Distillation for In-context Learning](#model-distillation-for-in-context-learning)
    - [Model Distillation for SFT](#model-distillation-for-sft)
  - [Model Merge](#model-merge)
- [Survey](#survey)
- [Others](#others)

## Length-Aware Guidance


### Prompt Guidance
> Prompt guidance methods make LRMs generate less reasoning text directly by adding explicit length constraint instructions to the prompts.

#### Active Prompt Guidance
> Active Prompt Guidance methods add the explicit length constraint instructions set by users to the prompt of LRMs to generate short reasoning text.

| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.02 | **Chain of Draft: Thinking Faster by Writing Less** |   arXiv     | [link](https://arxiv.org/pdf/2502.18600) |        [link](https://github.com/sileix/chain-of-draft)      |
| 2025.02 | **s1: Simple test-time scaling** |   arXiv     | [link](https://arxiv.org/abs/2501.19393) |        [link](https://github.com/simplescaling/s1)     |
| 2024.07 | **Concise Thoughts: Impact of Output Length on LLM Reasoning and Cost** | arXiv | [link](https://arxiv.org/abs/2407.19825) | - |
| 2024.01 | **The Benefits of a Concise Chain of Thought on Problem-Solving in Large Language Models** |   arXiv     | [link](https://arxiv.org/abs/2401.05618) |        [link](https://github.com/matthewrenze/jhu-concise-cot)      |

#### Passive Prompt Guidance
> Passive Prompt Guidance methods rely on additional models or algorithms to generate explicit length constraint instructions corresponding to different data, rather than user-specified.


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2024.12 | **Token-Budget-Aware LLM Reasoning** | arXiv | [link](https://arxiv.org/abs/2412.18547) | [link](https://github.com/GeniusHTX/TALE) |


### Reward Guidance
> From the perspective of reinforcement learning, the reward guidance based method designs a reward function optimized for length to generate high-precision answers while reducing the consumption of reasoning tokens as much as possible.


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.03 | **DAPO: an Open-source RL System from ByteDance Seed and Tsinghua AIR** |   arXiv     | [link](https://dapo-sia.github.io/static/pdf/dapo_paper.pdf) |   [link](https://github.com/volcengine/verl/tree/gm-tyx/puffin/main/recipe/dapo)    |
| 2025.03 | **L1: Controlling How Long A Reasoning Model Thinks With Reinforcement Learning** | arXiv | [link](https://www.arxiv.org/pdf/2503.04697) | [link](https://github.com/cmu-l3/l1) |
| 2025.02 | **Training Language Models to Reason Efficiently** |   arXiv     | [link](https://arxiv.org/abs/2502.04463) |        [link](https://github.com/Zanette-Labs/efficient-reasoning)     |
| 2025.02 | **Demystifying Long Chain-of-Thought Reasoning in LLMs** |   arXiv     | [link](https://arxiv.org/abs/2502.03373) |        [link](https://github.com/eddycmu/demystify-long-cot)     |
| 2025.01 | **O1-Pruner: Length-Harmonizing Fine-Tuning for O1-Like Reasoning Pruning** |   arXiv     | [link](https://arxiv.org/abs/2501.12570) |        [link](https://github.com/StarDewXXX/O1-Pruner)     |
| 2025.01 | **Kimi k1.5: Scaling Reinforcement Learning with LLMs** |   arXiv     | [link](https://arxiv.org/abs/2501.12599) |        -     |



## Length-Agnostic Optimization

### Latent Space Compression
Latent space compression replaces reasoning token with latent space, allowing more flexible and efficient reasoning for LRMs.

| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.02 | **LightThinker: Thinking Step-by-Step Compression** |   arXiv     | [link](https://arxiv.org/abs/2502.15589) |        [link](https://github.com/zjunlp/LightThinker)      |
| 2025.02 | **SoftCoT: Soft Chain-of-Thought for Efficient Reasoning with LLMs** |   arXiv     | [link](https://arxiv.org/abs/2502.12134) |        [link](https://github.com/xuyige/SoftCoT)      |
| 2025.02 | **Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach** | arXiv | [link](https://arxiv.org/pdf/2502.05171) | [link](https://github.com/seal-rg/recurrent-pretraining) |
| 2025.02 | **Token Assorted: Mixing Latent and Text Tokens for Improved Language Model Reasoning** | arXiv | [link](https://arxiv.org/abs/2502.03275) | - |
| 2025.01 | **Efficient Reasoning with Hidden Thinking** | arXiv | [link](https://arxiv.org/abs/2501.19201) | - |
| 2024.12 | **Training Large Language Model to Reason in a Continuous Latent Space** | arXiv | [link](https://arxiv.org/pdf/2412.06769v2) | [link](https://github.com/facebookresearch/coconut) |
| 2024.12 | **Compressed Chain of Thought: Efficient Reasoning through Dense Representations** | arXiv | [link](https://arxiv.org/pdf/2412.13171) |    -   |
| 2024.09 | **Expediting and Elevating Large Language Model Reasoning via Hidden Chain-of-Thought Decoding** | arXiv | [link](https://arxiv.org/pdf/2409.08561) |    -   |
| 2024.05 | **From Explicit CoT to Implicit CoT: Learning to Internalize CoT Step by Step** | arXiv | [link](https://arxiv.org/pdf/2405.14838) | [link](https://github.com/da03/internalize_cot_step_by_step) |
| 2024.03 | **Quiet-STaR: Language Models Can Teach Themselves to Think Before Speaking** | arXiv | [link](https://arxiv.org/abs/2403.09629) | [link](https://github.com/ezelikman/quiet-star) |
| 2023.10 | **Think before you speak: Training Language Models With Pause Tokens** |   arXiv     | [link](https://arxiv.org/abs/2310.02226v3) |        -     |



### Routing Strategy
> The routing strategy methods assign different reasoning strategies to the data according to the difficulty or task of the data to simplify the overall reasoning output of the data.


#### Template Routing
> Template routing method usually simplify reasoning output of LRMs by selecting the appropriate reasoning template or reasoning paradigms for data with different task scenarios.


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.03 | **How Well do LLMs Compress Their Own Chain-of-Thought? A Token Complexity Approach** | arXiv | [link](https://arxiv.org/abs/2503.01141) | [link](https://github.com/Compressed-CoT/compressed-cot) |
| 2025.03 | **Sketch-of-Thought: Efficient LLM Reasoning with Adaptive Cognitive-Inspired Sketching** | arXiv | [link](https://arxiv.org/pdf/2503.05179v1) | [link](https://github.com/SimonAytes/SoT) |
| 2025.02 | **Meta-Reasoner: Dynamic Guidance for Optimized Inference-time Reasoning in Large Language Models** |   arXiv     | [link](https://arxiv.org/pdf/2502.19918) |        -      |



#### Solution Routing
> Solution routing based methods work by selectively pruning of solutions in the chain of thought generated by LRMs.


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.02 | **When More is Less: Understanding Chain-of-Thought Length in LLMs** |   arXiv     | [link](https://arxiv.org/abs/2502.07266) |        -    |
| 2025.02 | **Stepwise Informativeness Search for Improving LLM Reasoning** |   arXiv     | [link](https://arxiv.org/abs/2502.15335) |        [link](https://github.com/SiyuanWangw/Informativeness-Search)    |
| 2025.01 | **Think Smarter not Harder: Adaptive Reasoning with Inference Aware Optimization** |   arXiv     | [link](https://arxiv.org/abs/2501.17974) |        -     |



## Computation Routing
> Computation routing based methods usually simplify reasoning output of LRMs by allocating different computing resources to data with different difficulty.


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2024.12 | **Efficiently Serving LLM Reasoning Programs with Certaindex** |   arXiv     | [link](https://arxiv.org/abs/2412.20993) |        [link](https://github.com/hao-ai-lab/Dynasor)    |



### Model Distillation
> Model distillation based methods construct a well-designed dataset to apply model learning, like SFT/In-context Learning/Preference Learning, thereby simplifying the reasoning output of the LRMs.


#### Model Distillation for Preference Learning


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.03 | **DAST: Difficulty-Adaptive Slow-Thinking for Large Reasoning Models** |   arXiv     | [link](https://arxiv.org/abs/2503.04472) |        -    |
| 2025.02 | **Do NOT Think That Much for 2+3=? On the Overthinking of o1-Like LLMs** |   arXiv     | [link](https://arxiv.org/abs/2412.21187) |        -    |
| 2025.01 | **Kimi k1.5: Scaling Reinforcement Learning with LLMs** |   arXiv     | [link](https://arxiv.org/abs/2501.12599) |        -     |
| 2024.12 | **Token-Budget-Aware LLM Reasoning** | arXiv | [link](https://arxiv.org/abs/2412.18547) | [link](https://github.com/GeniusHTX/TALE) |


#### Model Distillation for In-context Learning


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.02 | **Stepwise Perplexity-Guided Refinement for Efficient Chain-of-Thought Reasoning in Large Language Models** |   arXiv     | [link](https://arxiv.org/abs/2502.13260) |        -      |
| 2024.01 | **The Benefits of a Concise Chain of Thought on Problem-Solving in Large Language Models** |   arXiv     | [link](https://arxiv.org/abs/2401.05618) |        [link](https://github.com/matthewrenze/jhu-concise-cot)     |
| 2023.05 | **Chain-of-Symbol Prompting Elicits Planning in Large Langauge Models** |   arXiv     | [link](https://arxiv.org/abs/2305.10276) |        [link](https://github.com/hanxuhu/chain-of-symbol-planning)    |

#### Model Distillation for SFT


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.05 | **Can Pruning Improve Reasoning? Revisiting Long-CoT Compression with Capability in Mind for Better Reasoning** | arxiv | [link](https://arxiv.org/abs/2505.14582) | - |
| 2025.03 | **InftyThink: Breaking the Length Limits of Long-Context Reasoning in Large Language Models** |   arXiv     | [link](https://arxiv.org/abs/2503.06692) |        -     |
| 2025.02 | **Self-Training Elicits Concise Reasoning in Large Language Models** |   arXiv     | [link](https://arxiv.org/abs/2502.20122) |        [link](https://github.com/TergelMunkhbat/concise-reasoning)    |
| 2025.02 | **TokenSkip: Controllable Chain-of-Thought Compression in LLMs** |   arXiv     | [link](https://arxiv.org/abs/2502.12067) |        [link](https://github.com/hemingkx/TokenSkip)     |
| 2025.02 | **CoT-Valve: Length-Compressible Chain-of-Thought Tuning** |   arXiv     | [link](https://arxiv.org/abs/2502.09601) |        [link](https://github.com/horseee/CoT-Valve)     |
| 2025.02 | **Stepwise Informativeness Search for Improving LLM Reasoning** |   arXiv     | [link](https://arxiv.org/abs/2502.15335) |        [link](https://github.com/SiyuanWangw/Informativeness-Search)    |
| 2025.02 | **CODI: Compressing Chain-of-Thought into Continuous Space via Self-Distillation** |   arXiv     | [link](https://arxiv.org/pdf/2502.21074) |        -      |
| 2024.12 | **C3oT: Generating Shorter Chain-of-Thought without Compromising Effectiveness** | arXiv | [link](https://arxiv.org/abs/2412.11664) | - |
| 2024.12 | **Verbosity-Aware Rationale Reduction: Effective Reduction of Redundant Rationale via Principled Criteria** | arXiv | [link](https://arxiv.org/abs/2412.21006) | - |
| 2024.12 | **Token-Budget-Aware LLM Reasoning** | arXiv | [link](https://arxiv.org/abs/2412.18547) | [link](https://github.com/GeniusHTX/TALE) |
| 2024.11 | **Can Language Models Learn to Skip Steps?** | arXiv | [link](https://arxiv.org/abs/2411.01855) | [link](https://github.com/tengxiaoliu/LM_skip) | 







### Model Merge
> Model merge based methods typically merge the parameters of two models with different reasoning styles to obtain an LRMs with inclusion of different reasoning styles.


| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.03 | **Unlocking Efficient Long-to-Short LLM Reasoning with Model Merging** |   arXiv     | [link](https://arxiv.org/pdf/2503.20641v1) |        [link](https://github.com/hahahawu/long-to-short-via-model-merging)     |
| 2025.01 | **Kimi k1.5: Scaling Reinforcement Learning with LLMs** |   arXiv     | [link](https://arxiv.org/abs/2501.12599) |        -     |



## Survey

| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.04 | **Efficient Reasoning Models: A Survey** | arXiv | [link](https://arxiv.org/pdf/2504.10903v1) | [link](https://github.com/fscdc/Awesome-Efficient-Reasoning-Models) |
| 2025.03 | **A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimodality, and Beyond** | arXiv | [link](https://arxiv.org/abs/2503.21614) | [link](https://github.com/XiaoYee/Awesome_Efficient_LRM_Reasoning) |
| 2025.03 | **Stop Overthinking: A Survey on Efficient Reasoning for Large Language Models** | arXiv | [link](https://arxiv.org/pdf/2503.16419v2) | [link](https://github.com/mapuna/Reasoning-LLMs) |



## Others

| Time | Title                                                      |  Venue  |                           Paper                            |                            Code                            |
| ---- | -------------------------------------------------------- | :-----: | :-------------------------------------------------------: | :-------------------------------------------------------: |
| 2025.06 | **Accelerated Test-Time Scaling with Model-Free Speculative Sampling** | arXiv | [link](https://arxiv.org/abs/2506.04708) | - |
| 2025.03 | **EAGLE-3: Scaling up Inference Acceleration of Large Language Models via Training-Time Test** | arXiv | [link](https://arxiv.org/pdf/2503.01840v1) | [link](https://github.com/SafeAILab/EAGLE) |
| 2025.02 | **LongSpec: Long-Context Speculative Decoding with Efficient Drafting and Verification** | arXiv | [link](https://arxiv.org/pdf/2502.17421) | [link](https://github.com/sail-sg/LongSpec) |
| 2024.12 | **Bag of Tricks for Inference-time Computation of LLM Reasoning** | arXiv | [link](https://arxiv.org/abs/2502.07191) | [link](https://github.com/usail-hkust/benchmark_inference_time_computation_LLM) |






## Contributors
<a href="https://github.com/Hongcheng-Gao" target="_blank"><img src="https://avatars.githubusercontent.com/u/96536860?v=4" alt="Hongcheng-Gao" width="72" height="72"/></a> 
<a href="https://github.com/xinlong-yang" target="_blank"><img src="https://avatars.githubusercontent.com/u/73691354?v=4" alt="xinlong-yang" width="72" height="72"/></a> 
<a href="https://github.com/yueliu1999" target="_blank"><img src="https://avatars.githubusercontent.com/u/41297969?s=64&v=4" alt="yueliu1999" width="72" height="72"/></a> 
<a href="https://github.com/ColorDavid" target="_blank"><img src="https://avatars.githubusercontent.com/u/57055043?v=4" alt="ColorDavid" width="72" height="72"/></a> 
<a href="https://github.com/junming-yang" target="_blank"><img src="https://avatars.githubusercontent.com/u/60545459?v=4" alt="junming-yang" width="72" height="72"/></a> 
<a href="https://github.com/yili-19" target="_blank"><img src="https://avatars.githubusercontent.com/u/61128160?v=4" alt="yili-19" width="72" height="72"/></a> 



























