# MLP for Sequence Labeling

This project implements a **Multi-Layer Perceptron (MLP)** model for sequence tagging tasks. It follows the workflow used in the accompanying notebook `2nd_Assignment_POS_tagging_MLP.ipynb`.

---

## About
Implements a Multi-Layer Perceptron (MLP) for MLP, word embeddings. Includes preprocessing (tokenization, vocabulary/OOV handling), training with mini-batches, and evaluation on a held-out test set.

---

## Features

- Data preprocessing: tokenization, vocabulary creation, OOV handling
- Model: word embeddings (optional), fully connected layers with non-linear activations, dropout
- Training loop with batching and early stopping (if implemented in notebook)
- Evaluation: accuracy on held-out set and per-class metrics (confusion matrix if available)
- Reproducible runs with fixed seeds (if set in notebook)

---

## Example

**Input sentence**  
`The quick brown fox jumps over the lazy dog .`

**Predicted tags (example)**  
`DET ADJ ADJ NOUN VERB ADP DET ADJ NOUN PUNCT`

---

## Usage

1. Install dependencies (adjust to your environment):
   ```bash
   pip install torch datasets matplotlib scikit-learn
   ```

2. Open the notebook and run all cells:
   ```bash
   jupyter notebook MLP_ex10.ipynb
   ```

3. The notebook will:
   - load and preprocess the dataset,
   - train the MLP model,
   - report evaluation metrics.

---

## Future Work

- Compare with RNN/BiLSTM and Transformer baselines
- Use contextualized embeddings (e.g., ELMo/BERT) as features
- Hyperparameter search (learning rate, hidden size, dropout)

---

## References

- Universal Dependencies (UD) Treebanks
- Jurafsky & Martin — Sequence Labeling
