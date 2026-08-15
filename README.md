# A-Machine-learning-based-web-Appilcation-firewall-WAF-
A Machine Learning-Based Web Application Firewall (WAF) detects and blocks malicious web traffic using signature-based rules and a Random Forest model. It identifies attacks such as SQL Injection and XSS, provides explainable security decisions, and classifies requests as Allowed, Quarantined, or Blocked.
# Machine Learning-Based Web Application Firewall (WAF)

An intelligent Web Application Firewall that combines signature-based detection and machine learning to identify and block malicious web traffic in real time, with Explainable AI (XAI) for transparency.

## Features

- Signature-Based Detection
  Detects common attacks like SQL Injection, XSS, LFI, and Command Injection using regex patterns.

- Machine Learning Detection
  Uses a Random Forest model to identify anomalous and obfuscated payloads.

- Explainable AI (XAI)
  Provides human-readable explanations for each decision: Blocked, Quarantined, or Allowed.

- Interactive Dashboard UI
  Real-time testing panel to simulate attacks and view responses instantly.

- Logging System
  Tracks blocked requests, quarantined requests, and allowed traffic.

- Adaptive Thresholding
  Dynamically adjusts detection sensitivity based on attack patterns.

## Tech Stack

- Backend: Python, Flask
- Machine Learning: Scikit-learn (Random Forest)
- Frontend: HTML, CSS, JavaScript
- Other: Regex, Feature Engineering, REST APIs

## How It Works

1. Incoming request is captured.
2. Signature engine checks for known attack patterns.
3. ML model analyzes payload features such as entropy, token patterns, and special characters.
4. A risk score is calculated.
5. The request is classified as Allowed, Quarantined, or Blocked.
6. XAI generates an explanation for the decision.

## How to Run

git clone https://github.com/lalualfaz/ai-firewall.git
cd ai-firewall
pip install flask scikit-learn numpy joblib
python app.py

## Admin Access

URL: http://127.0.0.1:8080/login
Username: admin
Password: adminpass

## Demo

- SQL Injection: Blocked
- XSS Attack: Blocked
- Normal Request: Allowed
- High Entropy Payload: Quarantined

## Limitations

- Trained on a synthetic dataset
- No real threat intelligence integration
- Designed for learning and demonstration purposes

## Future Improvements

- Real-world traffic datasets
- Cloud deployment
- SIEM integration
- Rate limiting and IP blocking

## Author

Your Name
AG
