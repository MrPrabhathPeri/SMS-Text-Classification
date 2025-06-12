# 📱 SMS Spam Detection using LSTM

This project is a text classification model built using TensorFlow and LSTM layers to detect spam messages from SMS data. It uses a dataset provided by freeCodeCamp.

## 🚀 How It Works

- Downloads and loads SMS training and validation data from `.tsv` files.
- Preprocesses text data using TensorFlow Datasets' `SubwordTextEncoder`.
- Pads sequences to a uniform length for input into the neural network.
- Builds a sequential model with:
  - `Embedding` layer for word vector representation.
  - `Bidirectional LSTM` for learning sequence patterns.
  - Dense layers for classification.
- Trains the model and evaluates on a validation set.
- Includes a function to make predictions on custom messages.

## 🧾 Dataset

- Train: [train-data.tsv](https://cdn.freecodecamp.org/project-data/sms/train-data.tsv)
- Test: [valid-data.tsv](https://cdn.freecodecamp.org/project-data/sms/valid-data.tsv)

Each message is labeled either:
- `ham` (not spam)
- `spam`

## 📦 Requirements

Install the dependencies using the following commands:

```bash
pip install tf-nightly tensorflow-datasets pandas matplotlib
```

## 🛠 How to Run

```python
# Clone or download this script and run in Google Colab or any Python environment.

# Automatically installs necessary packages and downloads the dataset
!pip install tf-nightly tensorflow-datasets
!wget https://cdn.freecodecamp.org/project-data/sms/train-data.tsv
!wget https://cdn.freecodecamp.org/project-data/sms/valid-data.tsv
```

Run the complete code block to:
- Load and preprocess data
- Train the model
- Evaluate predictions using the `test_predictions()` function

## ✅ Example Predictions

```python
predict_message("how are you doing today")               # ham
predict_message("you have won £1000 cash!")              # spam
predict_message("sale today! call 98912460324")          # spam
```

## 🏁 Final Test Output

```text
You passed the challenge. Great job!
```

## 📚 Concepts Used

- Natural Language Processing (NLP)
- Sequence Modeling
- Bidirectional LSTM
- Binary Classification
- TensorFlow & Keras
- Subword Tokenization


