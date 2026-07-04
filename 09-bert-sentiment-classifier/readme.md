# BERT Sentiment Classifier

A Deep Learning and Natural Language Processing (NLP) pipeline for multiclass sentiment analysis (positive, neutral, negative) using a fine-tuned BERT (`bert-base-uncased`) model via Hugging Face Transformers.

## Features
* Language Detection: Automated language filtering using `langid`.
* NLP Data Cleaning: Strips URLs, hashtags, user mentions, and digits using Regex.
* Tokenization & Dataset Management: Tokenized via `BertTokenizer` with active padding and dynamic truncation mapping using the Hugging Face `datasets` library.
* Model Training: Multi-class classification fine-tuning with `Trainer` and `TrainingArguments` (hyperparameter tracking, checkpoint saving, and evaluation metrics tracking).
* Inference Pipeline: A function that handles raw text tokenization, computes softmax probabilities, and outputs the predicted sentiment class.

## Quick Start
```bash
   pip install torch transformers datasets pandas sklearn langid
```

---