## 

## Week1: Generative AI use cases, project lifecycle, and model pre-training

##### Learning Objectives

- Discuss model pre-training and the value of continued pre-training vs fine-tuning
- Define the terms Generative AI, large language models, prompt, and describe the transformer architecture that powers LLMs
- Describe the steps in a typical LLM-based, generative AI model lifecycle and discuss the constraining factors that drive decisions at each step of model lifecycle
- Discuss computational challenges during model pre-training and determine how to efficiently reduce memory footprint
- Define the term scaling law and describe the laws that have been discovered for LLMs related to training dataset size, compute budget, inference requirements, and other factors.

##### Lab 1 - Generative AI Use Case: Summarize Dialogue

There is a dialogue summarization task using generative AI, showing the way that how the input text affects the output of the model, and perform prompt engineering to direct it towards the task you need. By comparing zero shot, one shot, and few shot inferences, people will understand the prompt engineering and see how it can enhance the generative output of Large Language Models.

---

## Week2: Fine-tuning and evaluating large language models

##### Learning Objectives

- Describe how fine-tuning with instructions using prompt datasets can improve performance on one or more tasks
- Define catastrophic forgetting and explain techniques that can be used to overcome it
- Define the term Parameter-efficient Fine Tuning (PEFT)
- Explain how PEFT decreases computational cost and overcomes catastrophic forgetting
- Explain how fine-tuning with instructions using prompt datasets can increase LLM performance on one or more tasks

##### Lab 2 - Fine-tune a generative AI model for dialogue summarization

In this notebook, an existing LLM from Hugging Face for enhanced dialogue summarization will be fine-tuned. The FLAN-T5 model, which provides a high quality instruction, will be used to tune model and summarize text out of the box. To improve the inferences, a full fine-tuning will also be explored to approach and evaluate the results with ROUGE metrics. Then people can perform PEFT fine-tuning, evaluate the resulting model and see that the benefits of PEFT outweigh the slightly-lower performance metrics.

---

## Week3: Reinforcement learning and LLM-powered applications

##### Learning Objectives

- Describe how RLHF uses human feedback to improve the performance and alignment of large language models
- Explain how data gathered from human labelers is used to train a reward model for RLHF
- Define chain-of-thought prompting and describe how it can be used to improve LLMs reasoning and planning abilities
- Discuss the challenges that LLMs face with knowledge cut-offs, and explain how information retrieval and augmentation techniques can overcome these challenges

##### Lab 3 - Fine-tune FLAN-T5 with reinforcement learning to generate more-positive summaries

In this jupyter notebook, a FLAN-T5 model will be fine-tuned to generate less toxic content by Facebook's hate speech reward model. The reward model is a binary classifier that predicts either "not hate" or "hate" for the given text. Proximal Policy Optimization (PPO) will be used to fine-tune and detoxify the model.
