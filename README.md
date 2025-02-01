# Apply topsis to find best pre-trained model for Text Conversational 🧠🤖

A comprehensive evaluation framework for comparing pre-trained conversational AI models using multiple NLP metrics.**This project builds on and integrates components from my [previous project of Topsis](https://github.com/Sumit0504/Topsis_Sumit_102203514) for evaluation.**

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
| ![result](https://github.com/user-attachments/assets/c801b622-333d-4274-a5db-88f4e1322741)
 | Contains average scores for ROUGE, F1, Perplexity, etc. per model |
| ![final](https://github.com/user-attachments/assets/e8e09988-7ede-441a-b8e1-c2c882a50b96)
 | Final ranking using TOPSIS (Technique for Order Preference by Similarity) |
| ![topsis_models_comparison](https://github.com/user-attachments/assets/f659a736-043b-432c-aee0-14a5f97587f1)
 | Visual comparisons of individual metrics across models |
|ROUGE-1_comparison, ROUGE-2_comparison, ROUGE-L_comparison, Response Length_comparison, Response Length, Perplexity:Bar graphs comparing individual metrics.
![ROUGE-1_comparison](https://github.com/user-attachments/assets/110472c3-bc5a-4488-a548-ee4f6360deb1)
![ROUGE-2_comparison](https://github.com/user-attachments/assets/13cc8fac-45e5-44ed-a463-5731b3f70b5c)
![ROUGE-L_comparison](https://github.com/user-attachments/assets/a2fc4f65-2566-46c9-9a21-147e64d1d35d)
![Response Length_comparison](https://github.com/user-attachments/assets/20052f02-25a0-41cc-bbf3-cd5411263964)
![Perplexity_comparison](https://github.com/user-attachments/assets/3a740775-f844-4bf7-bf8d-2421f7dedc63)

|
 
## Dependencies ⚙️
- Python 3.7+
- Core: `nltk`, `torch`, `transformers`
- Metrics: `rouge-score`, `bert-score`, `sklearn`
- Visualization: `matplotlib`, `pandas`

Install all requirements:
```bash
>> pip install -r requirements.txt
>> python -m nltk.downloader popular  # Download NLTK data
```
**Final Thought**:  
This work demonstrates how systematic evaluation—combined with iterative reuse of past projects—can accelerate NLP research. By openly sharing this framework, I hope to empower developers to make data-driven decisions when choosing conversational AI models. Contributions and extensions are welcome! 🚀
