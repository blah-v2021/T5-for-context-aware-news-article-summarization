## (1) Description: 

The internet is flooded with news articles daily, making it difficult for readers to consume and process long pieces of information.
Summarization helps compress these articles into concise summaries without losing the core message.
The project explores how state-of-the-art NLP models, particularly T5, can be used to automatically generate high-quality summaries of Indian news articles.
The solution aims to be language-aware, context-sensitive, and scalable for real-world news summarization applications.

## (2) Duration:
Feb 2025- April 2025

## (3) Methodology:

- Dataset Preparation 
Source: Custom CSV file with 4500+ Indian news articles and human-written summaries.
Preprocessing:
Lowercasing, cleaning special characters.
Tokenization using T5Tokenizer.
Appended "summarize: " prefix to each article as required by the T5 model.

- Model Training 
Base Model: t5-small from HuggingFace Transformers.
Fine-Tuning Environment: Google Colab (GPU), PyTorch.
Key Libraries: HuggingFace Transformers, W&B for experiment tracking.

- Training Strategy 
Used Seq2SeqTrainer from HuggingFace.
Monitored loss, validation performance.
Optimized with AdamW and a learning rate scheduler.
Logging with WandB for transparency and analysis.
