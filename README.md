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

 ### Deep Learning Models
   - 1D CNN (Raw Protein Sequence)
   - Hybrid CNN + ESM + SVC

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


## Research Findings

- ESM embeddings significantly outperformed traditional TF-IDF approaches.
- Increasing ESM training samples improved model generalization.
- CNN performance improved considerably with higher epochs.
- Hybrid CNN + ESM architecture did not outperform standalone ESM + SVC.
- Results suggest that pretrained transformer embeddings capture protein semantics more effectively than raw sequence CNN learning alone.

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

# protein-function-prediction
>>>>>>> 32c297ff1df91bdac12205c68502053a52438873
