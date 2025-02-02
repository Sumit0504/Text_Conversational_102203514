# Apply topsis to find best pre-trained model for 🧠🤖

A comprehensive evaluation framework for comparing pre-trained conversational AI models using multiple NLP metrics. **This project builds on and integrates components from my [previous project of topsis] (https://github.com/Sumit0504/Topsis_Sumit_102203514) for evaluation.**

## Overview 📌
This project evaluates 6 pre-trained conversational models (like DialoGPT variants) on 5 diverse prompts to assess:
- **Response quality** (ROUGE, F1-Score)
- **Fluency** (Perplexity, Response Length)
- **Grammatical correctness** 
- **Ranking** (TOPSIS methodology)

---

## Integration with Previous Work 🔄
This project leverages code and methodologies from my **[previous NLP evaluation project](link_to_previous_project_repo)**:
1. **Shared Components**:
   - **Metric Calculation**: ROUGE, F1, and perplexity logic reused with minor adaptations for conversational responses.
   - **Visualization Pipeline**: Code for plotting metrics (e.g., `matplotlib` templates) directly imported.
   - **TOPSIS Ranking**: Ranking algorithm from prior work applied here for model comparison.

2. **Enhancements**:
   - Added support for **conversational-specific metrics** (e.g., response length analysis).
   - Integrated **Hugging Face models** instead of custom-trained summarization models.
   - Improved visualization readability for multi-model comparisons.

---

## Project Structure 🌳 (Updated)

- **evaluate_models.py: Main script for evaluating language models and performing analysis. -results.csv: CSV file containing detailed evaluation results.**
- **topsis.csv: CSV file containing TOPSIS analysis results.**
- **topsis_BarGraph: Bar graph visualizing TOPSIS scores.**


---

## Key Files 📄
| File | Description |
|------|-------------|
| ![result](https://github.com/user-attachments/assets/31eb5963-42f0-4470-bfbc-5a579d63054c)
 | Contains average scores for ROUGE, F1, Perplexity, etc. per model |
| ![final](https://github.com/user-attachments/assets/cec1ca3e-78e7-40e3-ae64-40bf84e85be9)
 | Final ranking using TOPSIS (Technique for Order Preference by Similarity) |
| ![topsis_models_comparison](https://github.com/user-attachments/assets/13ef83dd-6c04-45e1-bf39-f84b38b39b26)
 | Visual comparisons of individual metrics across models |
|ROUGE-1_comparison, ROUGE-2_comparison, ROUGE-L_comparison, Response Length_comparison, Response Length, Perplexity:Bar graphs comparing individual metrics.
![ROUGE-1_comparison](https://github.com/user-attachments/assets/45bf1a7d-eb54-45c6-ae32-0ed45c52552b)
![ROUGE-2_comparison](https://github.com/user-attachments/assets/1ef357e4-18ab-4fc8-a928-70c3b5155229)
![ROUGE-L_comparison](https://github.com/user-attachments/assets/5a7ec9b8-78c4-4cbb-b3c9-84afe369f65c)
![Response Length_comparison](https://github.com/user-attachments/assets/c8fc93a4-c5b2-47a7-a7df-975661714ddc)
![ROUGE-L_comparison](https://github.com/user-attachments/assets/776c7495-71f2-48bf-bdfa-fa774aebd6c5)
|
 ---
## Dependencies ⚙️
- Python 3.7+
- Core: `nltk`, `torch`, `transformers`
- Metrics: `rouge-score`, `bert-score`, `sklearn`
- Visualization: `matplotlib`, `pandas`
---
## Install all requirements:
```bash
pip install -r requirements.txt
python -m nltk.downloader popular  # Download NLTK data
```
---
## Final Thought:

This work demonstrates how systematic evaluation—combined with iterative reuse of past projects—can accelerate NLP research. By openly sharing this framework, I hope to empower developers to make data-driven decisions when choosing conversational AI models. Contributions and extensions are welcome! 🚀

---
