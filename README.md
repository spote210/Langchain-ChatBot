# Langchain-ChatBot
🤖 Chatbot Using Neural Networks
This project demonstrates how to build a simple rule-based chatbot using a feedforward neural network model in Python with PyTorch. It includes data preprocessing, model training, and inference to respond to user input based on intent classification.

## 📁 Files
1-chatbots.ipynb — Jupyter notebook with all steps: data loading, preprocessing, model definition, training, and testing.

intents.json — JSON file with training data: tags, patterns (inputs), and responses (output).

## 🧠 Key Components
Data Preparation

Loads intents from a JSON file.

Tokenizes and stems words.

Converts patterns to Bag-of-Words vectors.

### Model Architecture

A simple Feedforward Neural Network (FFNN) built with PyTorch.

Input size = vocabulary size, output size = number of intents.

### Training

CrossEntropyLoss and Adam optimizer used.

Trains the model on labeled intent data.

Saving Model

Trained model and metadata (input size, output size, vocabulary) are saved to data.pth.

Inference (Chatbot)

Loads the trained model.

Accepts user input and returns appropriate response based on intent prediction.

## ⚙️ How to Run
Clone this repository or copy the notebook.

Ensure you have PyTorch, nltk, and numpy installed.

Run all cells in the notebook.

Type messages in the chatbot interface at the bottom of the notebook.

## 📦 Requirements
Python 3.7+

PyTorch

NLTK

NumPy

## Install dependencies with:

bash
Copy
Edit
pip install torch nltk numpy
🔍 Example Usage
plaintext
Copy
Edit
You: Hi
Bot: Hello, how can I help you?

You: Bye
Bot: See you later, have a nice day!
## 📚 Credits
Based on classic intent classification datasets.

## Uses PyTorch for deep learning implementation.
