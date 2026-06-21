# 🛡️ Phishing URL Detector

A Python-based cybersecurity tool that detects phishing and suspicious URLs using rule-based logic like keyword detection, HTTPS check, WHOIS domain age analysis, and blacklist matching.

---

## ⚙️ Commands Used

### 1. Update System Packages
sudo apt update && sudo apt upgrade -y

---

### 2. Install Python & Pip
sudo apt install python3 python3-pip -y

---

### 3. Create Project Folder
mkdir phishing-url-detector  
cd phishing-url-detector  

---

### 4. Create Files
touch phishing_detector.py blacklist.txt report.txt README.md  

---

### 5. Create Virtual Environment
python3 -m venv venv  

---

### 6. Activate Virtual Environment
source venv/bin/activate  

---

### 7. Install Dependencies
pip install python-whois requests  

---

### 8. Run Project
python3 phishing_detector.py  

---

## 🧪 Test URLs Used

### 🚨 Phishing URLs
http://login-verify-bank-security.xyz  
http://secure-gift-win.net  
http://bank-update-alert-login.com  
http://paypal-security-login.xyz  

---

### ✅ Safe URLs
https://www.google.com  
https://www.wikipedia.org  
https://github.com  
https://www.paypal.com  

---

## 💻 Example Output

Enter URL: http://login-verify-bank-security.xyz  
⚠️ High Risk Phishing Website  

Enter URL: https://www.google.com  
✅ Safe Website  

---

## 📁 Project Structure

phishing-url-detector/  
│  
├── phishing_detector.py  
├── blacklist.txt  
├── report.txt  
└── README.md  

---

## 🧠 Project Summary

- Built a Python-based phishing URL detection tool  
- Used rule-based detection techniques  
- Implemented keyword + HTTPS + WHOIS + blacklist logic  
- Tested with real phishing and safe URLs  
- Learned cybersecurity fundamentals (SOC basics)

---

## 🚀 Skills Used

- Python Programming  
- Cyber Security Basics  
- URL Threat Detection  
- OSINT (WHOIS concept)  
- Linux (Kali)

---

## ⚠️ Disclaimer

This project is for educational purposes only.
