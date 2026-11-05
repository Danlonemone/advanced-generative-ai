# Advanced Generative AI

Coursework on large language models and generative models: tokenization and embeddings, retrieval-augmented generation (RAG), knowledge graphs, parameter-efficient fine-tuning (LoRA/PEFT), preference optimization (DPO), reinforcement learning (GRPO), GANs, and VAEs.

All notebooks were run in **Google Colab** (mostly on a T4 GPU) and are shown here **with their original outputs**.

## Highlights
- **[LoRA Fine-Tuning for Software Vulnerability Detection](lora_vulnerability_detection.ipynb)**: fine-tunes TinyLlama-1.1B with LoRA to classify C functions from the Devign (CodeXGLUE) dataset as vulnerable or safe. Covers preprocessing, token-length analysis, stratified sampling and evaluation.
- **[Retrieval-Augmented Generation](Assignment_3_RAG-1.ipynb)**: a RAG pipeline built with LangChain, a Chroma vector store, MiniLM embeddings and Phi-3-mini, served through a Gradio interface.
- **[GRPO Fine-Tuning](Assignment_7_GRPO-1.ipynb)**: reinforcement-learning fine-tuning on GSM8K math reasoning with custom reward functions for answer correctness and format.

## Notebooks
| Notebook | Topic |
|---|---|
| [Assignment 1: Introduction to Language Models](Assignment%201_%20Introduction%20to%20Language%20Models.ipynb) | Loading and prompting Phi-3 with Hugging Face pipelines |
| [Assignment 2: Tokens and Token Embeddings](Assignment2_Tokens_and_Token_Embeddings.ipynb) | Comparing LLM tokenizers; contextual embeddings |
| [Assignment 3: RAG](Assignment_3_RAG-1.ipynb) | LangChain + Chroma + Phi-3 retrieval QA with a Gradio UI |
| [Assignment 4: Fine-Tuning LLMs](Assignment_4_Fine_Tuning_of_LLMs-1.ipynb) | Supervised fine-tuning with Hugging Face TRL and PEFT |
| [Assignment 5: Neo4j](Assignment_5__Neo4j.ipynb) | Graph database with Cypher queries and embeddings on a healthcare dataset |
| [Assignment 6: DPO](Assignment_6_DPO-1.ipynb) | Direct Preference Optimization on the Human-Like DPO dataset |
| [Assignment 7: GRPO](Assignment_7_GRPO-1.ipynb) | GRPO reinforcement learning on GSM8K with Unsloth |
| [Assignment 8: LLM Fine-Tuning for Docker Commands](Assignment_8_LLM_FineTuning_DockerCmd-1.ipynb) | SFT of Llama-3.2-1B to turn natural language into Docker commands |
| [Assignment 9: WGAN-GP](Assignment_9_WGAN_GP.ipynb) | Wasserstein GAN with gradient penalty on Oxford Flowers 102 (PyTorch) |
| [Assignment 10: VAE](Assignment%2010_VAE_MNIST.ipynb) | Variational autoencoder generating MNIST digits (Keras) |
| [LoRA Vulnerability Detection](lora_vulnerability_detection.ipynb) | TinyLlama + LoRA on the Devign dataset |

Data file: `healthcare.csv` (used by Assignment 5).

## Tech stack
Python · PyTorch · TensorFlow/Keras · Hugging Face Transformers, Datasets, PEFT, TRL · Unsloth · LangChain · ChromaDB · Gradio · Neo4j · scikit-learn · Matplotlib

## Notes
- Paths like `/content/drive/...` refer to Google Drive mounted in Colab.
- In the Neo4j notebook, the database password was replaced with a placeholder before publishing.
- Colab's saved widget metadata was rewrapped in the standard `state` format so GitHub can preview the notebooks. Code cells and outputs are unchanged.
- If a large notebook doesn't preview on GitHub, open it on [nbviewer](https://nbviewer.org/) instead.
