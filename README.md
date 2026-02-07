# 🚀 Civo# 🌾 AgriAssist — Smart Agriculture Assistant

AgriAssist is a full-stack web application that helps farmers and agriculture researchers make data-driven decisions. It provides:

* 🌱 Crop yield prediction
* 💧 Irrigation recommendation
* 🌦 Weather information
* 📊 Machine learning–based insights

The project consists of a Python backend API and a simple web frontend interface.

---

## 📁 Project Structure

```
AgriAssist/
│
├── backend/
│   ├── datasets/
│   ├── models/
│   ├── routes/
│   ├── main.py
│   └── requirements.txt
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── app.js
│
├── docs/
└── resources/
```

---

## 🚀 Features

* Crop yield prediction using ML models
* Irrigation recommendation system
* Weather API integration
* REST API backend
* Interactive frontend dashboard following civora Nexus guidelines
* CSV dataset processing
* Modular and scalable architecture

---

## 🛠 Tech Stack

### Backend

* Python
* FastAPI
* Scikit-learn
* Pandas
* Uvicorn

### Frontend

* HTML
* CSS
* JavaScript (Vanilla JS)

---

## ⚙️ Setup Guide

## 1. Install Required Software

### Install Python

1. Download Python from: [https://www.python.org/downloads/](https://www.python.org/downloads/)

2. During installation, enable:

   ```
   ✔ Add Python to PATH
   ```

3. Verify installation:

   ```
   python --version
   ```

---

## 2. Backend Setup

### Step 1: Open Project in VS Code

Open the project folder in VS Code.

### Step 2: Navigate to Backend Folder

```
cd backend
```

### Step 3: Create Virtual Environment

```
python -m venv venv
```

Activate it:

**Windows:**

```
venv\Scripts\activate
```

### Step 4: Install Dependencies

```
pip install -r requirements.txt
```

### Step 5: Train MOdel

For yield model :
```
python models/irrigation_model.py
```
For irrigation model :
```
python models/yield_model.py
```

### Step 6: Run Backend Server

```
uvicorn main:app --reload
```

Backend runs at:

```
http://127.0.0.1:8000
```

API documentation:

```
http://127.0.0.1:8000/docs
```

---

## 3. Frontend Setup

### Step 1: Open Frontend Folder

```
cd frontend
```

### Step 2: Run Using Live Server

Recommended method:

1. Install Live Server extension in VS Code
2. Right-click `index.html`
3. Click Open with Live Server

Frontend opens in browser automatically.

---

## ▶️ How to Use

1. Start the backend server
2. Open the frontend in browser
3. Enter required agriculture inputs
4. View predictions and recommendations

---

## 🔌 API Endpoints

### Crop Yield Prediction

```
POST /yield/predict
```

### Irrigation Recommendation

```
POST /irrigation/predict
```

### Weather Data

```
GET /weather
```

You can test endpoints using the built-in FastAPI Swagger UI:

```
http://127.0.0.1:8000/docs
```

---

## ❗ Common Issues & Fixes

### Backend not starting

* Make sure Python is installed
* Ensure virtual environment is activated
* Reinstall dependencies:

  ```
  pip install -r requirements.txt
  ```

### Port already in use

Run backend on another port:

```
uvicorn main:app --reload --port 8001
```

### Frontend not connecting to backend

Check that:

* Backend server is running
* API base URL in `app.js` matches backend address

---

## 📈 Future Improvements

* User authentication
* Database integration
* Advanced ML models
* Mobile responsive UI
* Deployment to cloud

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍🌾 Author

Nitin Agrawal

---

## ⭐ Support

If you find this project useful, consider giving it a star on GitHub!
