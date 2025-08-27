
# 🎓 Student Exam Performance Predictor  

This project is a **Machine Learning application** built using **Python and Flask**, deployed on an **AWS EC2 instance**, that predicts a student's **Math score** based on various input features such as gender, ethnicity, parental education level, lunch type, test preparation course, writing score, and reading score.  

The model was trained on a dataset of student performance and saved for real-time predictions via a user-friendly web interface.  

---

## 🚀 Project Overview  

- **Frontend**: HTML templates rendered with Flask (form-based UI).  
- **Backend**: Flask server handling input requests and making predictions using the trained ML model.  
- **ML Model**: Trained on student exam performance dataset using **CatBoost** and preprocessing pipelines.  
- **Deployment**: Hosted on an **AWS EC2 instance** for global accessibility.  

🔮 **Goal**: Predict a student's **Math score** from demographic details and prior exam scores.  

---

## ⚙️ Features  

✅ User-friendly UI to input student details  
✅ Predicts **Math scores** instantly  
✅ Flask-based REST API backend  
✅ Pre-trained ML model with preprocessing pipeline  
✅ Deployed on **AWS EC2** for production use  

---

## 🧑‍💻 Tech Stack  

- **Programming Language**: Python 3  
- **Framework**: Flask  
- **Machine Learning**: CatBoost, Scikit-learn  
- **Frontend**: HTML, CSS (Flask templates)  
- **Deployment**: AWS EC2 (Linux, Gunicorn/Flask)  

---

## 🔧 Installation & Setup  

### 1. Clone the Repository  
```bash
git clone https://github.com/krishmaniyar/Student-Exam-Predictor.git
cd student-exam-predictor
```

### 2. Create Virtual Environment  
```bash
python -m venv venv
source venv/bin/activate   # For Linux/Mac
venv\Scripts\activate      # For Windows
```

### 3. Install Dependencies  
```bash
pip install -r requirements.txt
```

### 4. Run the Application Locally  
```bash
python application.py
```

App will be available at:  
👉 `http://51.20.189.64:5000/`  

---

## ☁️ Deployment on AWS EC2  

1. Launch an EC2 instance (Ubuntu).  
2. SSH into instance:  
3. Install Python, pip, and Git.  
4. Clone this repo and set up a virtual environment.  
5. Run Flask app using **Gunicorn** or directly:  
   ```bash
   gunicorn -w 4 application:app -b 0.0.0.0:5000
   ```  
6. Open EC2 security group and allow inbound traffic on port `5000`.  
7. Access app via:  
   👉 `http://51.20.189.64:5000/`  

---

## 📊 Dataset  

The dataset used contains student performance details:  
- **Gender**  
- **Race/Ethnicity**  
- **Parental Level of Education**  
- **Lunch Type**  
- **Test Preparation Course**  
- **Reading Score**  
- **Writing Score**  

**Target Variable**: Math Score  

---

## 🤝 Contributing  

1. Fork this repository  
2. Create your feature branch (`git checkout -b feature-name`)  
3. Commit changes (`git commit -m 'Add feature'`)  
4. Push to branch (`git push origin feature-name`)  
5. Open a Pull Request  

---

⚡ **Author**: *Krish*  
💡 Built with Python, Flask, and Machine Learning 🚀  
