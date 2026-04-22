# LSTM-Based Text Generation Model

## Overview

This project implements a text generation model using LSTM (Long Short-Term Memory) networks. The model is trained on a dataset of ~3000 sentences and is capable of predicting the next word as well as generating complete sentences from a given seed text.

---

## Objectives

* Learn sequence modeling using LSTM
* Build a next-word prediction system
* Generate human-like sentences from a seed input
* Understand tokenization and sequence padding

---

## Model Architecture

* Embedding Layer
* LSTM Layer(s)
* Dense Output Layer (Softmax)

---

## Dataset

* ~3000 sentences
* Preprocessed using:

  * Tokenization
  * Sequence generation
  * Padding

---

## Features

### 1. Next Word Prediction

Predicts the next word given an input sequence.

```python
seed_text = "life is"
next_word = predictor(model, tokenizer, seed_text, max_sequence_length)
```

Output:

```
Input Text: life is
Next Word: a
```

---

### 2. Sentence Generation

Generates a sequence of words starting from a seed text.

```python
generate_text(model, tokenizer, "life is about", 10, max_sequence_length)
```

Output:

```
life is about accepting the challenges along the way choosing to keep moving
```

---

## Model Performance

* Accuracy: ~76%
* Trained on a relatively small dataset, showing decent generalization

---

## Key Learnings

* How LSTMs handle sequential dependencies
* Importance of tokenization and padding
* Trade-off between dataset size and model performance
* Difference between word-level vs sentence-level generation

---

## Tech Stack

* Python
* TensorFlow / Keras
* NumPy
* Pandas

---

## Future Improvements

* Train on larger datasets
* Compare with GRU and Transformer models
* Add temperature-based sampling
* Deploy as a web application

---

## How to Run

```bash
git clone <repo-link>
cd lstm-text-generator
pip install -r requirements.txt
```

Run the notebook or script to train and test the model.

---

## Contributing

Feel free to fork and improve the project.

---

## License

Add a license if you plan to open-source this project.
