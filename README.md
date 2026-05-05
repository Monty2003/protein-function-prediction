<<<<<<< HEAD
# Protein Function Prediction using ML & ESM

## Overview
This project predicts protein function (enzyme, binding, transport) from amino acid sequences using machine learning and deep learning embeddings.

## Features
- Protein sequence preprocessing (FASTA → CSV)
- k-mer based feature engineering
- TF-IDF vectorization
- Multiple ML models (LR, RF, SVM)
- ESM pretrained embeddings (transformers)
- Model comparison and performance scaling
- Final accuracy: ~94%

## Dataset
- Swiss-Prot (Reviewed dataset from UniProt)
- Balanced dataset created from raw sequences

## Models Used
### Classical ML
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)

### Advanced Model
- ESM embeddings + SVC (Best)

## Results
| Model | Accuracy |
|------|--------|
| TF-IDF + SVM | 91% |
| ESM + SVC | 94% |

## Tech Stack
- Python
- Scikit-learn
- Biopython
- HuggingFace Transformers
- PyTorch

## How to Run
1. Clone repo
2. Install requirements:
   ```bash
   pip install -r requirements.txt
=======
# protein-function-prediction
>>>>>>> 32c297ff1df91bdac12205c68502053a52438873
