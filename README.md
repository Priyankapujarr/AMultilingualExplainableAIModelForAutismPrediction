# A Multilingual Explainable AI Model For Autism Prediction
# 🧠 Multilingual Explainable Model for Autism Prediction

This project is a web-based system designed to support early screening of Autism Spectrum Disorder (ASD) in children. It integrates behavioral screening, facial image analysis, MRI scan interpretation, multilingual chatbot assistance, and explainable AI — all within a simple, interactive interface.

---

## 🚀 Features

- ✅ *Behavioral Questionnaire Prediction* (0–3 & 4–11 years)
- 🖼 *Facial Image Prediction* using TensorFlow Lite CNN
- 🧠 *MRI Image Prediction* using Keras CNN model
- 💬 *Multilingual Chatbot* (English, Hindi, Kannada) for guidance
- 🤖 *Explainable AI Integration* via Gemini API
- 🌐 *Flask-based web interface* for real-time user interaction
- 🎙 *Voice Input Support* using Speech Recognition API
- 🌍 *Language Translation* using Google Translate API

---

## 📁 Project Structure
├── app.py                      # Main Flask application
├── templates/
│   ├── index.html              # Homepage
│   ├── chatbot.html            # English chatbot UI
│   ├── chatboth.html           # Hindi chatbot UI
│   └── chatbotk.html           # Kannada chatbot UI
├── static/
│   ├── testmri/                # MRI image uploads
│   └── testface/               # Facial image uploads
├── models/
│   ├── 0-3.sav                 # Logistic Regression model (0–3 yrs)
│   ├── 4-11.sav                # Logistic Regression model (4–11 yrs)
│   ├── face_model.tflite       # TFLite model for facial prediction
│   ├── mri_model.h5            # Keras CNN model for MRI
│   └── class_names.pkl         # Class labels
└── requirements.txt            # Python dependencies
---

## 🧪 How It Works

1. *User selects a module* (form, image, MRI, or chatbot)
2. *Input is submitted* (text or image)
3. *Preprocessing*:
   - Behavioral inputs are encoded
   - Images are resized, normalized, and reshaped
4. *Model is loaded*:
   - .sav for forms, .tflite for face, .h5 for MRI
5. *Prediction is made*
6. *Explanation generated via Gemini*
7. *Result + reason + chatbot support is displayed*

---

## 🖥 Installation

```bash
git clone https://github.com/yourusername/autism-prediction.git
cd autism-prediction
pip install -r requirements.txt
python app.py
⚙ Requirements
	•	Python 3.10
	•	Flask
	•	TensorFlow
	•	Keras
	•	Scikit-learn
	•	OpenCV
	•	Googletrans
	•	Gemini API key (for XAI & chatbot)
	•	Web browser (Chrome/Firefox)
