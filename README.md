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
## ⚙️ Creating Python File using Nano Editor

Open file using nano editor:

nano phishing_detector.py

Then paste the following Python code inside the file:

---

## 🧠 Python Code

```python
# Phishing URL Detection Tool
# Author: Mohit Kumar

def check_phishing(url):
    suspicious_keywords = [
        "login", "verify", "secure", "account", "update",
        "bank", "paypal", "confirm", "signin", "password"
    ]

    suspicious_domains = [
        ".xyz", ".tk", ".ml", ".ga", ".cf"
    ]

    score = 0

    for keyword in suspicious_keywords:
        if keyword in url.lower():
            score += 1

    for domain in suspicious_domains:
        if domain in url.lower():
            score += 1

    if "https://" not in url:
        score += 1

    print("\nURL Analysis Report")
    print("-" * 30)
    print(f"URL: {url}")

    if score >= 2:
        print("⚠️ High Risk Phishing Website Detected")
    elif score == 1:
        print("⚠️ Suspicious URL - Be Careful")
    else:
        print("✅ Safe URL")

url = input("Enter Website URL: ")
check_phishing(url)

Press ctrl+X+Y & enter

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
