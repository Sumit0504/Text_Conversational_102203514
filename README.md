# Apply topsis to find best pre-trained model for Text Conversational 🧠🤖

![TOPSIS Ranking](topsis_models_comparison.png)

A comprehensive evaluation framework for comparing pre-trained conversational AI models using multiple NLP metrics.

## Overview 📌
This project evaluates 6 pre-trained conversational models (like DialoGPT variants) on 5 diverse prompts to assess:
- **Response quality** (ROUGE, F1-Score)
- **Fluency** (Perplexity, Response Length)
- **Grammatical correctness** 
- **Ranking** (TOPSIS methodology)

Designed for NLP practitioners to compare model performance objectively.

## Project Structure 🌳
- **Evaluation Script: The main script (evaluate_models.py) contains the code for evaluating the language models using BLEU, ROUGE, and TOPSIS analysis.**

- Results: **The results of the evaluation are stored in CSV files (results.csv and topsis.csv).**

- Graphs: **Bar graphs comparing TOPSIS scores and individual metrics (BLEU, ROUGE-1, ROUGE-2, ROUGE-L, and Response Length) are saved as PNG files.**



## Key Files 📄
| File | Description |
|------|-------------|
| /Users/mac/Documents/Text_Conversational_102203514/final.csv | Runs model evaluation, calculates metrics, and generates results/plots |
| `results.csv` | Contains average scores for ROUGE, F1, Perplexity, etc. per model |
| `final.csv` | Final ranking using TOPSIS (Technique for Order Preference by Similarity) |
| `*_comparison.png` | Visual comparisons of individual metrics across models |

## Dependencies ⚙️
- Python 3.7+
- Core: `nltk`, `torch`, `transformers`
- Metrics: `rouge-score`, `bert-score`, `sklearn`
- Visualization: `matplotlib`, `pandas`

Install all requirements:
```bash
pip install -r requirements.txt
python -m nltk.downloader popular  # Download NLTK data