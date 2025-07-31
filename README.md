
# Research Task 5 – Descriptive Statistics & LLM Reasoning  
**Syracuse University iSchool – OPT Research Project**

## Objective

This project explores how Large Language Models (LLMs) like ChatGPT can reason about real-world datasets when prompted with natural language questions. Specifically, it evaluates whether LLMs can interpret, reason, and respond correctly to questions about the **2025 Syracuse Women’s Lacrosse team statistics**, which were extracted from a publicly available PDF.

## What This Repo Contains

- A Jupyter Notebook (`task_05_descriptive_statistics.ipynb`) that:
  - Parses and cleans a PDF dataset
  - Converts it into a structured CSV
  - Queries ChatGPT using OpenAI’s Python SDK (`gpt-3.5-turbo`)
  - Displays answers to various analytical questions

- A list of prompts used with the LLM and evaluation notes

## Files Included

| File            | Description                                           |
|-----------------|-------------------------------------------------------|
| `task_05_descriptive_statistics.ipynb`    | Full notebook for PDF parsing, CSV conversion, and LLM interaction |
| `prompts.txt`   | List of prompts asked to the LLM                     |
| `README.md`     | This documentation file                              |


## 📊 Questions Asked to LLM

Examples of natural language queries posed to ChatGPT:

- How many games did Syracuse Women’s Lacrosse play in 2025?
- What is their win/loss record?
- Which game had the highest attendance?
- What was their average goal score?
- Which game was the closest by goal margin?

## Steps to Run the Notebook

1. Install dependencies:
   ```bash
   pip install openai PyPDF2 pandas
   ```

2. Replace your OpenAI API key in the notebook cell:
   ```python
   client = OpenAI(api_key="YOUR_KEY_HERE")
   ```

3. Launch Jupyter Notebook in your terminal:
   ```bash
   jupyter notebook
   ```

4. Open `task_05_descriptive_statistics.ipynb` from the Jupyter UI and run all cells.

## Evaluation Strategy

Each LLM-generated answer was validated using:
- Raw calculations from the dataset (using Pandas)
- Manual inspection of output
- Prompt engineering to retry or rephrase questions if the initial answer was incorrect or vague
