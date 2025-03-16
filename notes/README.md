# Generative AI with LangChain Notes

## Introduction

Generative AI refers to algorithms that can generate novel content as opposed to analyzing or acting on existing data like the more traditional, predictive machine learning systems.

- **MMLU (Massive multitask language understanding) Benchmark:** A comprehensive evaluation framework testing large language models (LLMs) on **57 diverse tasks** across STEM, humanities, and social sciences, using **multiple-choice questions** to assess knowledge and reasoning from elementary to graduate levels.
- **Zero-Shot, One-Shot, Few-Shot Learning:** Techniques used to evaluate models on tasks with varying levels of provided context:
  - **Zero-Shot:** No examples, tests inherent generalization.
  - **One-Shot:** One example, tests minimal learning ability.
  - **Few-Shot (e.g., 5-shot):** Few examples, tests pattern recognition and adaptability.
- **Purpose of Both:** MMLU evaluates general knowledge and reasoning, while zero/few-shot tests assess a model’s ability to generalize and adapt to new tasks with minimal guidance.
- **GPTs (Generative Pre-trained Transformers):** Large language models based on the **Transformer architecture** designed for text understanding and generation.
  - Pretrained on massive datasets using **unsupervised learning**.
  - Focus on **next-word prediction** to understand context.
  - Scalable with billions to trillions of parameters.
- **Multimodal models** are machine learning models designed to process and integrate data from multiple modalities (different types of input, such as text, images, audio, and video) to perform various tasks. These models aim to combine information from diverse sources for a richer understanding and more robust decision-making.
- **Perplexity** is a metric used to evaluate the performance of language models, especially in natural language processing (NLP). It measures how well a model predicts a sequence of words. A lower perplexity indicates that the model is better at predicting the text. It works just like the English word.
- NVIDIA’s CUDA platform allows direct programming of GPUs which has been crucial for deep learning algorithms. Many LLM papers describe the use of NVIDIA A100s for training.
- Representation learning is about a model learning its internal representations of raw data to perform a machine learning task, rather than relying only on engineered feature extractions.
