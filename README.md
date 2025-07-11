# AMDFINAL
# AMD Project: Detecting Similar Reviews Using MinHash and LSH

This project was developed as part of the course Algorithms for Massive Data in the Master in Data Science for Economics at the University of Milan.

## Objective

The goal of this project is to detect and filter near-duplicate book reviews in the Amazon Books Reviews dataset using scalable techniques. Two main approaches were implemented and compared:

- Brute-force Jaccard similarity on tokenized word sets
- MinHash combined with Locality-Sensitive Hashing (LSH) for scalable candidate generation

## Contents

- AMD_final_Zhaksylyk.ipynb — Jupyter Notebook with the full implementation
- AMD_projectReport_Zhaksylyk.pdf — Final project report written in LaTeX
- README.md — Project description

## Dataset

The dataset used is publicly available on Kaggle:

Amazon Books Reviews — mohamedbakhet/amazon-books-reviews  
https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews

It contains approximately 300,000 book reviews, including review text, rating, user identifiers, and metadata.

## Tools and Libraries

- Python: pandas, nltk, matplotlib
- datasketch: for MinHash and LSH indexing
- Jupyter Notebook
- LaTeX (Overleaf): for report writing and formatting

## Performance Summary (10,000 reviews sample)

| Metric                        | Brute-force Jaccard | MinHash + LSH |
|------------------------------|---------------------|----------------|
| Candidate pairs evaluated    | 49,995,000          | 467            |
| Final similar pairs (≥ 0.5)  | 238                 | 235            |
| Execution time (seconds)     | 385                 | 16             |

## Author

Zhaksylyk Tansykbay  
Master in Data Science for Economics  
University of Milan  
Academic Year: 2024/2025
