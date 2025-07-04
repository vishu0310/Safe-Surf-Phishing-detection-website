# 🛡️ SafeSurf – Phishing Detection Website

![Python](https://img.shields.io/badge/Python-3.8-blue)
![Flask](https://img.shields.io/badge/Backend-Flask-green)
![ML](https://img.shields.io/badge/ML-RandomForest-yellow)
![License](https://img.shields.io/badge/License-MIT-blue)

**SafeSurf** is an intelligent and user-friendly phishing detection website built to **identify malicious URLs** in real-time using **machine learning** and **URL-based feature analysis**. The platform aims to empower users to browse the internet more safely by flagging suspicious websites before they cause harm.

> 🔍 Detects Phishing URLs | 🧠 ML-Powered | 🌐 Real-Time & Easy-to-Use

---

![Home Page](https://github.com/user-attachments/assets/ecf6f91f-7319-4092-a254-c21dc4292166)

---

## 🌟 Features

- 🔗 **URL Scanning**: Input any website URL and instantly check if it's malicious.
- 🧠 **Machine Learning Detection**: Trained ML model analyzes features like URL length, presence of IPs, special characters, redirection behavior, and more.
- 📊 **Probability Score**: Get a risk score with prediction confidence.
- ✅ **Safe & Simple UI**: Minimal, modern interface with clear results.
- 🚨 **Warning Alerts**: Red flags shown for suspicious domains.
- 🌐 **WHOIS & SSL Checks** *(planned)*

---

## 🏗️ Tech Stack

| Layer         | Technologies                                |
|---------------|---------------------------------------------|
| **Frontend**  | HTML, CSS, JavaScript, Bootstrap            |
| **Backend**   | Flask (Python), REST API                    |
| **ML Model**  | scikit-learn, pandas, NumPy, joblib         |
| **Dataset**   | PhishTank, Alexa Top Sites, Custom Features |
| **Hosting**   | Render / Heroku (or local deployment)       |

---

## 🧠 ML Model Overview

![ML Graph](https://github.com/user-attachments/assets/3f294a15-8e2e-4fd6-8111-8f5f146306e5)

- **Type**: Binary Classification (Phishing vs Legitimate)
- **Best Model**: Random Forest Classifier
- **Key Features**:
  - Length of URL
  - Use of `@` or `//`
  - Presence of `https`
  - Number of subdomains
  - Domain age, redirection tags, and iframes
  - WHOIS/DNS-based checks *(optional)*

---

## 🖼️ Screenshots

| Homepage                        | Detection Result                 |
|--------------------------------|----------------------------------|
| ![Homepage](https://github.com/user-attachments/assets/ecf6f91f-7319-4092-a254-c21dc4292166) | ![ML Output](https://github.com/user-attachments/assets/3f294a15-8e2e-4fd6-8111-8f5f146306e5) |

---

## 📂 Project Structure

```bash
Safe-Surf-Phishing-detection-website/
├── static/              # CSS, JS, assets
├── templates/           # HTML templates (Jinja2)
├── phishing_model.pkl   # Trained ML model
├── app.py               # Flask server
├── feature_extract.py   # Extracts URL features
├── requirements.txt     # Python dependencies
└── README.md


🚀 How to Run Locally
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/vishu0310/Safe-Surf-Phishing-detection-website.git
cd Safe-Surf-Phishing-detection-website
2. Set up a virtual environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Run the Flask app
bash
Copy
Edit
python app.py
Open your browser at 👉 http://localhost:5000

✍️ Author
Vishu Patle
GitHub • LinkedIn

📃 License
This project is licensed under the MIT License

🔮 Future Enhancements
✅ WHOIS & SSL certificate validation

✅ Real-time browser extension (Chrome/Firefox)

✅ Integration with Google Safe Browsing & PhishTank API

✅ Progressive Web App (PWA) for mobile

🤝 Contributions
Contributions, suggestions, and PRs are welcome!
Feel free to fork the repo and help improve SafeSurf 🛡️
