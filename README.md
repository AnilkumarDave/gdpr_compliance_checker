# 🛡️ GDPR Compliance Checker (Academic Project – MSc Information Security & Digital Forensics)

📅 **Project Duration:** 25 November 2022 – 5 December 2022 (≈ 10 days, Part-Time)  
🎓 **Academic Year:** First Term (MSc Information Security & Digital Forensics)  
🏛️ **Institution:** University of East London, London, UK  
📘 **Subject:** Security Management  

---

## 🏫 Project Overview

This project was developed as an extra-curricular academic activity during my MSc studies in **Information Security & Digital Forensics**.  

It is a **Python-based GDPR Compliance Checker** designed to evaluate small websites or datasets for potential data privacy and GDPR violations.  
The tool automatically scans webpages, identifies personal data collection points, and generates structured reports with compliance recommendations.

### This project demonstrates understanding of:
- GDPR principles and lawful data processing  
- Privacy risk assessment and reporting  
- Python-based automation and web scraping  

> **Note:** All websites and data used in this project were dummy, publicly available, or created for testing purposes only.  
> No real personal or institutional data was accessed or stored.

---

## 🎯 Project Objectives

- Identify and analyse personal data collection points (e.g., forms, emails, phone numbers).  
- Evaluate websites or datasets against key GDPR principles (Art. 5 & 6).  
- Generate structured compliance reports with findings and recommendations.  
- Provide a simple, automated method for educational GDPR compliance checks.  
- Demonstrate data protection awareness through practical analysis.  

---

## ⚙️ Modernisation Note

| Originally Built | Modernised & Uploaded |
|------------------|------------------------|
| Nov–Dec 2022 | Oct 2025 |

**Modern updates include:**
- ✅ Updated Python code for Python 3.13  
- ✅ Improved report generation (CSV & Excel summaries)  
- ✅ Added compliance scoring system  
- ✅ Enhanced error handling and data validation  
- ✅ Refined layout and comments for clarity  
- ✅ Modern README documentation and version control setup  

---

## 🧩 System Features

### 👨‍💻 Core Features
- Crawl and scan target website for personal data indicators.  
- Detects:
  - Form fields (name, email, phone, address, etc.)
  - Contact details (emails, phone numbers)
  - Non-HTTPS content or insecure data transmission  
- Generates:
  - Detailed **CSV** report of all findings  
  - **Excel** summary report with compliance score and recommendations  

---

## 📊 Report Output

| **Field** | **Description** |
|------------|----------------|
| **Page** | URL of scanned page |
| **Issue** | Type of GDPR concern (e.g., phone detected, form field) |
| **Value** | Data or field name found |
| **Result** | Flagged / Detected |
| **Recommendation** | Suggested action for compliance |
| **Legal Reference** | GDPR Article(s) |
| **Priority** | High / Medium |

---

## 📂 Project Files

| **File** | **Description** |
|-----------|----------------|
| `gdpr_compliance_checker.py` | Main Python script for scanning and report generation |
| `gdpr_report_full.csv` | Detailed output report of detected issues |
| `gdpr_report_summary.xlsx` | Summarised compliance report |
| `README.md` | Project documentation |

---

## ⚠️ Limitations

| **Limitation** | **Description** | **Possible Improvement** |
|----------------|------------------|---------------------------|
| Limited website depth | Scans only a few linked pages | Add configurable depth and sitemap parsing |
| Static analysis only | Does not execute JavaScript or dynamic pages | Integrate Selenium or Playwright |
| Basic GDPR rule set | Focuses on key principles only | Expand detection with AI-driven text analysis |
| Dummy / test sites only | Real systems not used for ethical reasons | Apply under ethical review with consent |

---

## 🌟 Advantages

- ✅ Fully offline, open-source, and Python-based  
- ✅ Works on dummy or local HTML websites  
- ✅ Produces structured reports for documentation  
- ✅ Easy to adapt for educational or internal audits  
- ✅ Demonstrates cybersecurity awareness and data protection principles  

---

## ⏱️ Project Timeline

| **Date Range** | **Task** |
|----------------|----------|
| 25 Nov 2022 | Requirement analysis and project planning |
| 26–28 Nov 2022 | Python module development |
| 29–30 Nov 2022 | Website scanning logic and regex patterns |
| 1–3 Dec 2022 | Report generation and compliance scoring |
| 4 Dec 2022 | Testing and debugging |
| 5 Dec 2022 | Final documentation and submission |

---

## 🔮 Future Scope

- Integration with AI/NLP to detect privacy policy gaps  
- Development of browser-based dashboard for GDPR analysis visualization  
- Automated data mapping and consent validation  
- Integration with external GDPR API databases  
- Real-time website monitoring for privacy risks  

---

## 🚀 Quick Setup

```bash
# Clone repository
git clone https://github.com/<yourusername>/gdpr-compliance-checker.git
cd gdpr-compliance-checker

# Create virtual environment
python -m venv .venv

# Activate environment
.\.venv\Scripts\activate      # Windows
source .venv/bin/activate     # Linux / macOS

# Install dependencies
pip install -r requirements.txt

# Run the project
python gdpr_compliance_checker.py

Output files:

gdpr_report_full.csv
gdpr_report_summary.xlsx

🏆 Project Achievement

This project showcases practical understanding of:

GDPR regulations and privacy analysis

Python automation, data parsing, and reporting

Ethical handling of data

Documentation and version control (GitHub)

It reflects real-world application of security management principles within a controlled, academic context.

📜 Disclaimer

This project was created for academic and educational purposes only.
All websites and data used were dummy or public test resources.
No real personal or institutional data was accessed or stored.
Images and data used in reports are for demonstration and understanding only.

✨ Author

Name: Anilkumar Dave
Email: daveanil48@gmail.com

About: MSc Information Security & Digital Forensics graduate passionate about cybersecurity, privacy compliance, and Python-based automation.
