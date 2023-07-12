# Smart Summarizer
This repository contains the implementation and evaluation of a Smart Summarizer, which automatically generates summaries from text using extractive and abstractive approaches. The project explores different techniques for text summarization and compares their performance. The study focuses on two primary models: TextRank for extractive summarization and BART for abstractive summarization.

## Implementation
The project utilizes the CNN Daily Mail News dataset for training and evaluation. Data preprocessing is performed to clean the text, including removing duplicates, converting to lowercase, and eliminating stop words and extraneous punctuation. The implementation includes the following steps:

### Extractive Summarizer:
TextRank: The extractive summarizer applies the TextRank algorithm to rank sentences based on importance, using cosine similarity and word embeddings.
BERT: The BERT model is fine-tuned for extractive summarization using the CNN Daily Mail dataset. It selects important phrases to generate the summary.

### Abstractive Summarizer:
Seq2Seq: The Seq2Seq model with attention mechanism is implemented using the Keras library. It processes variable-length input sequences and produces output sequences.
BART: The pre-trained BART model, designed for text summarization, is utilized to generate abstractive summaries. It leverages both auto-regressive and denoising objectives during pre-training.
The models are evaluated using the ROUGE metric, which measures the quality of the summaries by assessing word overlap and common subsequences with reference summaries.

# Evaluation
The models are evaluated using the ROUGE metric, specifically ROUGE-1, ROUGE-2, and ROUGE-L. The ROUGE-1 measure calculates word overlap between system-generated and reference summaries. ROUGE-2 considers consecutive word pairs, while ROUGE-L calculates the longest common subsequence. The evaluation provides F1 scores, recall, and precision for each model.

# Results
Extractive Summarizer:
### TextRank: ROUGE-1 F1 score: 0.16, Recall: 0.19, Precision: 0.14
### BERT: ROUGE-1 F1 score: 0.32, Recall: 0.59, Precision: 0.22

Abstractive Summarizer:
### Seq2Seq: ROUGE-1 F1 score: 0.12, Recall: 0.08, Precision: 0.28
### BART: ROUGE-1 F1 score: 0.47, Recall: 0.53, Precision: 0.42

The results indicate that BERT outperforms TextRank in extractive summarization, demonstrating higher recall, precision, and F1 scores. BART surpasses Seq2Seq in abstractive summarization, achieving better recall, precision, and F1 scores.

# Discussion
The project provides insights into the performance and trade-offs of various text summarization models. BERT proves to be more effective than TextRank in extractive summarization, while BART outperforms Seq2Seq in abstractive summarization. However, the complexity and interpretability of models should also be considered when choosing a specific approach. Further research and experimentation are necessary to explore hybrid models, enhance model interpretability, and investigate pre-training strategies to improve performance.
