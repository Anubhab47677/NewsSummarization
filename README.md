# 📰 News Summarization using Seq2Seq with Attention

An abstractive text summarization project that generates concise summaries of news articles using a **Sequence-to-Sequence (Seq2Seq) Encoder-Decoder architecture with LSTM networks and Attention mechanisms**.

The project explores and compares **Bahdanau Attention** and **Luong Attention** for improving the model's ability to focus on relevant parts of long news articles while generating summaries.

---

## 📌 Project Overview

News articles can contain a large amount of information, making it difficult to quickly understand their main points.

This project aims to automatically generate meaningful and concise summaries from news articles using **Deep Learning and Natural Language Processing (NLP)**.

Unlike extractive summarization, which selects existing sentences from an article, this project performs **abstractive summarization**, allowing the model to generate new sentences that capture the core meaning of the original article.

---

## 🎯 Objectives

- Build an abstractive news summarization system.
- Implement a Seq2Seq Encoder-Decoder architecture.
- Use LSTM networks for sequence processing.
- Implement Attention mechanisms to improve contextual understanding.
- Compare Bahdanau and Luong Attention.
- Optimize important model hyperparameters.
- Evaluate generated summaries using ROUGE metrics.

---

## 🧠 Model Architecture

The project uses a **Sequence-to-Sequence (Seq2Seq) architecture** consisting of:

```text
                NEWS ARTICLE
                     │
                     ▼
             Text Preprocessing
                     │
                     ▼
              Tokenization
                     │
                     ▼
             ┌──────────────┐
             │    Encoder   │
             │     LSTM     │
             └──────┬───────┘
                    │
              Hidden States
                    │
                    ▼
              Attention Layer
          ┌─────────┴─────────┐
          │                   │
   Bahdanau Attention   Luong Attention
          │                   │
          └─────────┬─────────┘
                    │
                    ▼
             ┌──────────────┐
             │   Decoder    │
             │     LSTM     │
             └──────┬───────┘
                    │
                    ▼
             Generated Summary