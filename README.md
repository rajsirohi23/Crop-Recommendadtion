# 🌱 Crop Recommendation Web App

A Machine Learning-based web application that recommends the most suitable crop to grow based on environmental and soil conditions. This project uses a **Random Forest model** trained on agricultural data and is deployed using **Flask**.

---

## 🚀 Live Demo

🌐 Frontend: https://crop-recommendadtion.onrender.com

## 🚀 Features

* 🌾 Predicts best crop based on input parameters
* 🤖 Machine Learning model (Random Forest)
* 🌐 Interactive web interface using HTML, CSS, JavaScript
* ⚡ Fast and lightweight Flask backend
* ☁️ Deployed on Render

---

## 🧠 Tech Stack

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Flask (Python)
* **Machine Learning:** Scikit-learn (Random Forest)
* **Deployment:** Render

---

## 📊 Input Parameters

The model takes the following inputs:

* Nitrogen (N)
* Phosphorus (P)
* Potassium (K)
* Temperature (°C)
* Humidity (%)
* pH value
* Rainfall (mm)

---

## 🧪 Model Details

* Algorithm: Random Forest Classifier
* Library: Scikit-learn
* Model file: `crop_reco_model.pkl`

---

## 📁 Project Structure

```
Crop-Recommendation/
│
├── app.py
├── crop_reco_model.pkl
├── requirements.txt
├── runtime.txt
├── Procfile
│
├── templates/
│   └── index.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── main.js
```

---

## ⚙️ Installation & Setup

1. Clone the repository:

```
git clone https://github.com/your-username/Crop-Recommendation.git
cd Crop-Recommendation
```

2. Create virtual environment:

```
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

3. Install dependencies:

```
pip install -r requirements.txt
```

4. Run the app:

```
python app.py
```

5. Open in browser:

```
http://127.0.0.1:5000/
```

---

## 🌍 Deployment

This project is deployed on **Render** using:

* `gunicorn` for production server
* `runtime.txt` to specify Python version
* Environment variables for configuration

---

## 📸 Output

The app predicts the most suitable crop based on given inputs and displays it instantly on the web interface.

---

## 🎯 Future Improvements

* 🌦️ Integrate real-time weather API
* 📱 Make UI fully responsive
* 📊 Add data visualization dashboard
* 🌍 Multi-language support

---

## 👨‍💻 Author

**Raj Sirohi**

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and share it!
