# Description of repository

This repository contains the implementation for the Master's Thesis: "Detecting Context-Induced Mistakes in Large Language Models Using Hidden States." It provides a framework to detect when an LLM is misled by external incorrect context (hallucinations) by monitoring its internal activations.

## Key components

- Feature attribution validation (`Feature_Attribution.ipynb`): A "sanity check" proving that Integrated Gradients (IG) converge to analytical weights in linear regimes, justifying the use of interpretability tools.
- `news_dataset_100_noisy.csv`: Dataset used in feature attribution validation.
- Pop-ConflictQA (`PopQA_Detection.ipynb`): Implementation of the $\Delta\Delta$ metric and PIT-normalization to detect factual answer flips in open-ended questions in Llama-3, Qwen, and Gemma models.
- Strategy-ConflictQA detection (`StrategyQA_Boolean.ipynb`): Implementation of the $\Delta\Delta$ metric and PIT-normalization to detect factual answer flips in True/False questions in Llama-3, Qwen, and Gemma models.

