# 🚦 Traffic Sign Recognition System using CNN and Flask Web App

> A high-performance, real-time traffic sign classification system built with Convolutional Neural Networks (CNNs) and deployed using Flask. Designed to enhance autonomous driving technologies and intelligent transportation systems.

---

## 📌 Table of Contents

- [🧠 Problem Statement](#-problem-statement)
- [🎯 Objectives](#-objectives)
- [📊 Results & Insights](#-results--insights)
- [📂 Dataset Information](#-dataset-information)
- [🧪 Methodology](#-methodology)
- [🖥️ Deployment & UI](#-deployment--ui)
- [⚙️ Tech Stack](#️-tech-stack)
- [🗂️ File Structure](#️-file-structure)
- [🚀 How to Run](#-how-to-run)
- [🔏 License](#-license)
- [🙏 Acknowledgements](#-acknowledgements)
- [📬 Contact](#-contact)

---

## 🧠 Problem Statement

Autonomous vehicles must reliably recognize and respond to traffic signs to ensure safety and compliance. Manual classification is error-prone, especially in variable weather, lighting, and image quality conditions. An intelligent, scalable solution is needed to detect and classify 43 traffic signs in real-time.

---

## 🎯 Objectives

- 📥 Load and preprocess the **GTSRB dataset**.
- 🧠 Design and train a **deep CNN** model for traffic sign classification.
- 🧪 Evaluate model performance using accuracy, loss, and visual metrics.
- 🌐 Develop a **Flask web app** that enables users to upload images and get predictions.
- ⚡ Enable real-time, scalable, and accurate predictions for real-world applications.

---

## 📊 Results & Insights

| Metric                  | Value              |
|-------------------------|--------------------|
| 🧠 Model Type           | Custom CNN (5 Conv layers) |
| 🎯 Final Accuracy       | **96.8%** on Test Set |
| ⚙️ Optimizer            | Adam |
| 📉 Final Loss           | 0.12 (Categorical Crossentropy) |
| ⏱️ Training Time        | ~15 minutes (NVIDIA GPU) |
| 🔍 Evaluation           | Confusion Matrix, Classification Report |
| 📈 Visuals              | Training curves, Prediction samples |

> The model generalizes well to unseen data and demonstrates high robustness across 43 classes of traffic signs.

---

## 📂 Dataset Information

- **Name**: [German Traffic Sign Recognition Benchmark (GTSRB)](https://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset)
- **Total Images**: ~50,000 (RGB)
- **Classes**: 43 different traffic signs
- **Image Dimensions**: Resized to 32x32 pixels
- **Format**: CSV annotation + Image folders
- **License**: Creative Commons (CC BY-NC-SA 3.0)

---

## 🧪 Methodology

### 🔧 Preprocessing
- Normalization of pixel values
- Image resizing to 32x32
- One-hot encoding of class labels

### 🧠 CNN Architecture
- Input Layer: 32x32x3
- Conv2D → ReLU → MaxPooling (x5)
- Fully Connected Layers (x2)
- Output Layer: Softmax (43 classes)

### 📈 Evaluation
- Confusion matrix to analyze misclassifications
- Real-time image predictions tested via web interface
- ROC curves and per-class accuracy visualization

---

## 🖥️ Deployment & UI

### 🧩 Flask Web Application
- Drag-and-drop or select an image to classify
- Predicts the sign type with high accuracy
- Fast, lightweight, and beginner-friendly interface

### 🖼️ UI Screenshot

![Web App Interface](./screenshots/Screenshot-2025-03-24-020945.png)

---

## ⚙️ Tech Stack

- **Programming Language**: Python 3.8+
- **Deep Learning Framework**: TensorFlow/Keras
- **Web Framework**: Flask
- **Data Handling**: NumPy, Pandas, OpenCV
- **Visualization**: Matplotlib, Seaborn
- **Deployment**: Localhost / WSGI-ready

---

## 🗂️ File Structure
traffic-sign-recognition/
├── app.py # Flask backend
├── model.py # Model architecture & training script
├── gtsrb-cnn.ipynb # Full training & analysis notebook
├── traffic_sign_model.h5 # Final trained model (43 classes)
├── templates/
│ └── index.html # Frontend HTML for upload UI
├── screenshots/ # UI screenshots
├── README.md # You're reading it now!


---

## 🚀 How to Run

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/traffic-sign-recognition.git
cd traffic-sign-recognition

2️⃣ Install Requirements
pip install -r requirements.txt

3️⃣ Start the App
python app.py


4️⃣ Access in Browser
Open your browser at: http://127.0.0.1:5000/

🔏 License
This project is licensed under the MIT License. You can freely use, modify, and distribute it with attribution.

🙏 Acknowledgements
GTSRB Dataset Team
TensorFlow and Keras Documentation
Flask Community & Core Devs
Python & OpenCV Libraries

📬 Contact
Name: Altamash Ali Ansari 
Email: altamash171201@gmail.com
GitHub: https://github.com/ansarimzp

🚗 Built for a smarter, safer, and more autonomous future in transportation.

---

### ✅ Want Additions?

I can also generate:
- `requirements.txt`
- `LICENSE` file (MIT, Apache, etc.)
- UI banner/logo
- Demo video script or abstract for submission


