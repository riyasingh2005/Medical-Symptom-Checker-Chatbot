# 🤖 AI-Based Symptom Checker Chatbot

![License](https://img.shields.io/badge/license-MIT-blue.svg)

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
- [Contribution](#contribution)
- [License](#license)
- [Contact](#contact)

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

