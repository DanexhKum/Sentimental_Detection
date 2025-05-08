# Emotion Sentence Classifier 😄😢😡

This project is a multi-label emotion classifier that detects emotions from a given sentence using a fine-tuned `distilroberta-base` model. The emotions it can identify are:

- Anger
- Anticipation
- Disgust
- Fear
- Joy
- Sadness
- Surprise
- Trust

## 🧠 Model Architecture

The model is based on a transformer backbone (`distilroberta-base`) followed by:

- A mean pooling layer on the last hidden states
- A hidden linear layer with ReLU activation
- A final classification layer with sigmoid activation for multi-label prediction
- BCEWithLogitsLoss for training

## 📦 Requirements

- Python 3.7+
- PyTorch >= 1.11
- Transformers (🤗 Hugging Face)
- CUDA (optional, for GPU acceleration)

Install dependencies:

```bash
pip install torch transformers

Developed by: Dhanesh Kumar & Danish Nanjiani.
