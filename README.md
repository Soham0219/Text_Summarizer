# 📝 Text Summarizer using Encoder-Decoder with Additive Attention

This project implements a **Text Summarization** model using the **Encoder-Decoder architecture** with **LSTMs** and **Bahdanau (Additive) Attention** mechanism. The model is trained to generate abstractive summaries of input text, learning the context and structure of human-written summaries.

## 🔍 Overview

Text summarization is the task of generating a concise and fluent summary while preserving key information content and overall meaning. This project focuses on **abstractive summarization**, where the model generates new phrases, rather than simply extracting existing ones from the text.

### Architecture Highlights:
- **Encoder:** A multi-layer LSTM that encodes the input text into hidden states.
- **Attention:** Bahdanau (Additive) Attention computes context vectors for each output step by learning to attend to relevant encoder hidden states.
- **Decoder:** Another LSTM that uses attention to decode the context into the summary sequence.

## 📚 Dataset

- Used the **Inshorts News Dataset**.
- Preprocessing included:
  - Lowercasing
  - Removing special characters
  - Tokenization
  - Padding
  - Word-to-index conversion (using custom vocabulary or pretrained embeddings)

## 🏗️ Model Details

- **Embedding Layer:** Trained from scratch.
- **Encoder:** LSTM layers returning sequences and states.
- **Attention Layer:** Bahdanau Attention mechanism (Additive Attention).
- **Decoder:** LSTM with attention-weighted context vector.
- **Loss Function:** Sparse Categorical Crossentropy
- **Optimizer:** Adam

## 🧠 Key Learnings

- Implementation of Bahdanau Attention from scratch
- Handling of variable-length sequences using masking
- Training and inference techniques in sequence-to-sequence models
- Sequence padding and alignment issues in NLP

