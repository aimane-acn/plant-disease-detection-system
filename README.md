## 🌱 Plant Disease Detection System
   📌 Overview
This project is a **distributed system** for detecting and predicting plant diseases using **deep learning**.
It allows users to upload plant images and receive predictions, confidence scores, and treatment recommendations.
---
   🏗️ Architecture
The system is composed of two main services:

* **Web Gateway (Django)**
  Handles user interface, authentication, and requests

* **AI Service (gRPC + CNN)**
  Processes images using a trained deep learning model

* **Database (SQLite)**
  Stores users and analysis history

---

## ⚙️ Tech Stack

* Python
* Django
* gRPC
* PyTorch / TensorFlow
* HTML, CSS, Bootstrap
* SQLite

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/plant-disease-detection.git
cd plant-disease-detection
```

### 2. Create virtual environment & Install dependencies
* Each service must be installed separately :

  🔹 1. AI Service setup
```bash
cd ai_service
python -m venv venv
venv\Scripts\activate   # Windows
# source venv/bin/activate  # Mac/Linux
pip install -r requirements.txt
```

    🔹 2. Web Gateway setup
```bash
cd web_gateway
python -m venv venv
venv\Scripts\activate   # Windows
# source venv/bin/activate  # Mac/Linux
pip install -r requirements.txt
```

### 3. Run AI service

```bash
cd ai_service
python server.py
```

### 4. Run web server

```bash
cd web_gateway
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

---

## 🌐 Access

Open: http://127.0.0.1:8000

---

## 📂 Project Structure

```
ai_service/      # AI inference service (gRPC + CNN model)
web_gateway/     # Django web application
```

---

## ⚠️ Notes

* Start the AI service before the web server (ai_service before web_gateway)
* Use Python 3.10 or higher
* Each service has its own virtual environment
* Do not share dependencies between services

---

## 👥 Authors

* Aimane Achibane

---

⭐ If you like this project, consider giving it a star on GitHub!
