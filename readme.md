# Fynd AI Intern – Take Home Assignment

## Task 1: Yelp Rating Prediction using Prompt Engineering

This repository contains my solution for **Task 1** of the Fynd AI Intern take-home assignment.  
The goal of this task is to predict Yelp star ratings (1–5) from review text using **LLM prompting**, and to evaluate how different prompt designs affect performance and reliability.

---

## Approach

- Used a sampled subset (~200 rows) of the Yelp Reviews dataset
- Designed **three different prompting strategies**:
  1. Basic prompt
  2. Structured sentiment-based prompt
  3. Strict JSON-enforced prompt
- Evaluated each prompt on:
  - Prediction accuracy
  - JSON validity
  - Consistency and reliability

---

## Model & Tools

- **LLM Provider:** OpenRouter  
- **Model Used:** LLaMA 3.1 (8B Instruct)
- **Language:** Python
- **Libraries:** pandas, tqdm, python-dotenv

---

## Results Summary

| Prompt Version | Accuracy | JSON Validity |
|---------------|----------|---------------|
| Prompt V1 | ~69.5% | 100% |
| Prompt V2 | ~65.0% | 100% |
| Prompt V3 | ~62.5% | 100% |

The results show a clear trade-off between prediction flexibility and output reliability when designing prompts.

---

## How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
---
## Create a .env file with your OpenRouter API key:
```bash
   OPENROUTER_API_KEY=your_key_here
   ```
---
## Open and run:

```bash 
   task1_rating_prediction.ipynb
```
---