# Keyword Extraction Capstone Project

## Overview
This project explores automatic keyword extraction from text using two approaches: YAKE! (Yet Another Keyword Extractor) and BRYT. The goal is to generate meaningful, searchable tags from text slices, including online book summaries, academic abstracts, and open datasets. By replicating and analyzing these methods, this project establishes a baseline for keyword extraction performance and identifies ways to improve on existing techniques.

## Project Structure
keyword-extraction-capstone/
│
├── data/                   # Folder containing input text files or datasets
│   ├── book_summaries/
│   ├── abstracts/
│   └── processed/
│
├── notebooks/              # Jupyter notebooks
│   ├── yake_example.ipynb
│   └── bryt_example.ipynb
│
├── scripts/
│   ├── bryt_tfidf_extract.py
│   ├── bryt_ensemble_extract.py
│   └── utils.py
│
├── results/                # results
│
├── README.md               # Project documentation
└── requirements.txt        # Python dependencies

## Dependencies
Python 3.9+
Jupyter Notebook / Jupyter Lab
Libraries: yake, pandas, numpy, nltk, tensorflow, torch, matplotlib, scikit-learn
Install all dependencies via pip:

## How to Run
YAKE!
1. Place your text files in data/book_summaries/ or data/abstracts/.
2. Open notebooks/yake_example.ipynb.
3. Adjust the KeywordExtractor parameters:
`kw_extractor = yake.KeywordExtractor(lan="en", n=3, dedupLim=0.9, top=10)`
4. Run the notebook to extract keywords

## Results
Extracted keywords are saved in results/ as CSV files.
Visualizations such as bar charts and word clouds are generated to show the most relevant keywords per document.
Keywords can be sorted by relevance score and compared directly to the original text.