# 🎤 Voice Emotion Detection Web App using HuBERT & Flask

A real-time **Voice Emotion Detection Web Application** built using **Flask**, **PyTorch**, and **HuBERT Transformer Model**.  
This system allows users to **register, login, record/upload voice audio**, and detect the **emotion** present in speech with a confidence score.

---

## 📌 Project Overview

This project is designed to identify human emotions from voice recordings using a **pretrained HuBERT (Hidden-Unit BERT)** model for speech classification.

The application includes:

- User Registration & Login System
- Secure Password Storage
- Real-time Voice Emotion Detection
- Audio Conversion (WebM → WAV)
- Emotion Prediction with Confidence Score
- Flask Web Interface
- SQLite Database Support

This project is useful for:

- AI-based emotion recognition systems
- Mental health support tools
- Human-computer interaction systems
- Interview / speech behavior analysis
- Research in speech-based AI applications

---

## 🚀 Features

### 👤 User Authentication
- User registration with:
  - Name
  - Email
  - Phone
  - Password
- Secure password hashing using `werkzeug.security`
- Login / Logout functionality
- Session-based authentication

### 🎙 Voice Emotion Detection
- Accepts recorded browser audio
- Converts uploaded **WebM audio** to **WAV format**
- Uses **HuBERT sequence classification model**
- Predicts emotion from speech
- Displays **emotion label + confidence percentage**

### 🧠 Supported Emotion Classes
The model maps raw predicted labels into user-friendly emotions such as:

- Confident
- Neutral
- Angry
- Sad
- Fear
- Disgust
- Surprise

---

## 🛠️ Tech Stack

### Backend
- Python
- Flask
- SQLite

### Deep Learning / AI
- PyTorch
- Hugging Face Transformers
- HuBERT Model
- Wav2Vec2 Feature Extractor

### Audio Processing
- SoundFile
- PyDub
- FFmpeg (required for audio conversion)

### Frontend
- HTML
- CSS
- JavaScript
- Jinja2 Templates

---

## 📂 Project Structure

```bash
Voice-Emotion-Detection-Web-App-using-HuBERT-Flask/
│
├── app.py
├── database.db
├── README.md
│
├── models/
│   └── hubert_emotion/
│       ├── config.json
│       ├── preprocessor_config.json
│       ├── pytorch_model.bin
│       └── ...
│
├── static/
│   ├── css/
│   ├── js/
│   ├── images/
│   └── ...
│
├── templates/
│   ├── index.html
│   ├── login.html
│   ├── register.html
│   ├── about.html
│   ├── voice_emotion.html
│   └── ...
│
└── temp files (generated during prediction)
