# 🤖 AI-Based Symptom Checker Chatbot

An AI-powered chatbot designed to help users identify symptoms and get relevant health-related information. This chatbot uses **Natural Language Processing (NLP)** and a trained **Recurrent Neural Network (RNN)** to interpret user queries intelligently and provide informative responses.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Training the Model](#training-the-model)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)

---

## 🧠 Overview

This project is a custom-built **AI symptom checker chatbot** that allows users to input their symptoms in natural language and receive context-aware replies about possible conditions or nearby healthcare facilities. The chatbot leverages deep learning for understanding user intent and provides medically relevant responses using a trained RNN model and structured JSON-based intent classification.

---

## 🌟 Features

- Built with **Flask** for a lightweight web interface
- Supports **NLTK** for tokenization and bag-of-words NLP preprocessing
- **PyTorch RNN** for intent classification
- Suggests nearby **medical centers** using geolocation
- Easily customizable intents and training data

---

## 🚀 Installation

To run this chatbot locally, follow these steps:

### 1. Clone this repository:

```bash
git clone https://github.com/<your-username>/symptom-checker-chatbot.git
cd symptom-checker-chatbot
```
### 2. Create a virtual environment and activate it:
```bash
python -m venv venv
venv\Scripts\activate  # Windows
# source venv/bin/activate  # Linux/Mac
```

### 3. Install all required packages:
```bash
pip install -r requirements.txt
```

### 4. Download required files:
Ensure the following files are placed in the root project directory:

intents.json – Defines the chatbot's response patterns and labels.

data_rnn.pth – Pre-trained RNN model file.

medical_centers.json – Contains mock data of medical facilities.

💻 Usage
Once setup is complete, launch the app:

```bash
python app.py
```
Then open your browser and go to:

```bash
http://localhost:5000
```
You can now interact with the chatbot through the web interface.

🛠️ Training the Model
To update or customize the chatbot’s knowledge base:

Edit the intents.json file to add or modify symptoms, questions, and responses.

Retrain the model using:

```bash
python train.py
```
The model will generate a new data.pth file. Make sure to update the model filename in chat.py under the FILE variable accordingly.

<details> <summary>📁 Project Structure</summary>
graphql
Copy
Edit
├── app.py           # Main Flask application  
├── chat.py          # Core logic for predictions  
├── train.py         # RNN model training script  
├── nltk_utils.py    # NLP preprocessing helpers  
├── intents.json     # Intent definitions and sample data  
├── data_rnn.pth     # Trained model  
├── static/          # CSS and frontend files  
├── templates/       # HTML templates  
└── requirements.txt # Python dependencies  
</details>

## 📦 Dependencies
This project uses the following libraries:

Python 3.x

Flask

PyTorch

NLTK

Geocoder

Install all at once via:

```bash
pip install -r requirements.txt
```
