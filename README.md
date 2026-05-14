<<<<<<< HEAD
## Protein Function Prediction using Classical ML, ESM Embeddings, CNN and Hybrid Deep Learning Models

## Research Objective
This project explores multiple machine learning and deep learning approaches for protein function prediction using amino acid sequences.

The research investigates:

- Classical ML models with TF-IDF features
- Transformer-based ESM embeddings
- 1D CNN sequence learning
- Hybrid CNN + ESM architectures
- Comparative performance analysis
# Protein Function Prediction using ML & ESM

## Overview
This project predicts protein function (enzyme, binding, transport) from amino acid sequences using machine learning and deep learning embeddings.

## Features
- Protein sequence preprocessing (FASTA → CSV)
- k-mer based feature engineering
- TF-IDF vectorization
- Multiple ML models (Logistic Regression, Random Forest, SVM)
- ESM pretrained embeddings (transformers)
- Model comparison and performance scaling
- Final accuracy: ~94%

## Dataset
- Swiss-Prot (Reviewed dataset from UniProt)
- Balanced dataset created from raw sequences


 ### Models Used

### Classical Machine Learning
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)

### Deep Learning Models
- 1D Convolutional Neural Network (1D CNN)
- Hybrid CNN + ESM Model
- ESM + Self-Attention Neural Network

### Advanced Techniques
- 5-Fold Cross-Validation
- Ensemble Learning (ESM + SVC + Self-Attention)
- Homology-Based Label Diffusion

 
 ## Results
   | Model                        | Dataset Size | Accuracy |
   | ---------------------------- | ------------ | -------- |
   | TF-IDF + Logistic Regression | 15000        | 90%      |
   | TF-IDF + Random Forest       | 15000        | 88%      |
   | TF-IDF + SVM                 | 15000        | 91%      |
   | ESM + SVC                    | 1500         | 88%      |
   | ESM + SVC                    | 9000         | 93%      |
   | ESM + SVC                    | 15000        | 94%      |
   | 1D CNN (5 Epochs)            | 15000        | 83%      |
   | 1D CNN (5 Epochs)            | 21000        | 86%      |
   | 1D CNN (15 Epochs)           | 15000        | 91%      |
   | Hybrid CNN + ESM + SVC       | 15000        | 90%      |
   | ESM + Self-Attention         | 15000        | 93.97%   |
   | Ensemble (SVC + Self-Attention)|15000       | 94.57%   |
   | Homology-Based Label Diffusion |15000       | 94.20%   |

### Cross-Validation Results

- ESM + SVC (5-Fold CV): **93.68% ± 0.39%**
- ESM + Self-Attention (5-Fold CV): **93.59% ± 0.75%**



## Research Findings

- ESM embeddings significantly outperformed traditional TF-IDF approaches.
- Increasing ESM training samples improved model generalization.
- CNN performance improved considerably with higher epochs.
- Hybrid CNN + ESM architecture did not outperform standalone ESM + SVC.
- Results suggest that pretrained transformer embeddings capture protein semantics more effectively than raw sequence CNN learning alone.
- Self-attention successfully captured relationships among embedding dimensions.
- Ensemble learning achieved the highest overall accuracy.
- Homology-based label diffusion was implemented and evaluated but did not outperform the ensemble baseline.
- The final ensemble model is the strongest candidate for deployment and publication.

## CNN Epoch Analysis
 We analyzed the effect of training epochs on 1D CNN accuracy using a dataset size of 15,000 protein sequences.
 
| Epochs | Accuracy |
|--------|----------|
| 5      | 0.89     |
| 10     | 0.91     |
| 15     | 0.90     |

Observation:
- Accuracy improved until 10 epochs.
- After 10 epochs, performance saturated.
- 10 epochs provided the best balance between learning and overfitting.
## Results

| Model | Accuracy |
|------|--------|
| TF-IDF + SVM | 91% |
| ESM + SVC (15000 samples) | 94% |

## Tech Stack
 ### Programming & Environment
- Python
- Jupyter Notebook
 ### Bioinformatics & Data Processing
- Biopython
- Pandas
- NumPy
 ### Machine Learning
- Scikit-learn
- TF-IDF Vectorization
- Logistic Regression
- Random Forest
- Support Vector Classifier (SVC)
 ### Deep Learning
- PyTorch
- 1D Convolutional Neural Network (1D CNN)
 ### Transformer Models
- Hugging Face Transformers
- Facebook ESM2 Protein Language Model
 ### Visualization & Analysis
- Matplotlib
- Seaborn
 ### Model Persistence
- Joblib


## Visualizations
- Model comparison graphs
- Confusion matrices
- Accuracy scaling experiments
  
## How to Run
1. Clone repo
2. Install requirements:
   ```bash
   pip install -r requirements.txt
=======

## Notebook Workflow
1. 01_fasta_to_csv.ipynb
2. 02_esm_embeddings.ipynb
3. 03_cnn_model.ipynb
4. 04_hybrid_cnn_esm.ipynb

## Future Work
- Transformer fine-tuning
- Attention-based architectures
- LSTM and BiLSTM experiments
- Ensemble learning
- Protein family-level prediction
- Structure-aware embeddings

## Methodology

1. Convert FASTA protein sequences into structured CSV data.
2. Generate protein embeddings using the ESM2 transformer model.
3. Train classical machine learning and deep learning models.
4. Perform 5-fold cross-validation to verify model robustness.
5. Build an ESM + Self-Attention neural network.
6. Combine ESM + SVC and Self-Attention models using ensemble learning.
7. Apply homology-based label diffusion as a biologically inspired post-processing step.
8. Compare all models using accuracy, F1-score, confusion matrices, and classification reports.

# protein-function-prediction
>>>>>>> 32c297ff1df91bdac12205c68502053a52438873


1. Clone the repository:
```bash
git clone https://github.com/Monty2003/protein-function-prediction.git
