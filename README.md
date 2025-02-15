>>> # **Small Language Model: Character Prediction with PyTorch**  
>>> *A minimal implementation of a character-level language model using PyTorch.*  

---

## Overview  
This project demonstrates a simple RNN-based language model trained on the string `"hello"`. The model learns to predict the next character in a sequence, making it a foundational example for understanding sequence modeling and neural networks in NLP.  

---

## Directory Structure  

---

### Installation & Setup  
  1. **Prerequisites**:  
     - Python 3.8+  
     - PyTorch: Install via `pip install torch` or follow [official guide](https://pytorch.org/get-started/locally/).  
  
  2. **Run the Script**:  
     ```bash
     python Small_language_model.py

## Examples & Usage :

  ## Example 1: Predict Next Character

  start_str = "he"
  predicted_char = predict_next_char(model, start_str)
  print(f"After '{start_str}', the model predicts: '{predicted_char}'")
  ### Output: After 'he', the model predicts: 'l'
  -----------------------------------

  ### Example 2: Modify Sequence Length 
  -----------------------------------
  # Change seq_length to 2
  seq_length = 2
  X = []
  y = []
  for i in range(len(encoded_text) - seq_length):
      X.append(encoded_text[i:i+seq_length])
      y.append(encoded_text[i+seq_length])
  ### Retrain the model with new X and y
-----------------------------------
  ### Key Takeaways
  
  Character-Level Modeling: Suitable for small datasets or custom text.
  RNN Architecture: Captures sequential patterns but struggles with long-term dependencies.
  Extensibility: Replace RNN with LSTM/GRU or scale up the model for larger datasets.

-------------------------------------
### Acknowledgments

+ Inspired by [**Andrej Karpathy’s Char-RNN**](https://github.com/karpathy/char-rnn).
+ Built with [**PyTorch**](https://pytorch.org/).
