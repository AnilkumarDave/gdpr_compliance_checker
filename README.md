# 🛡️ GDPR Compliance Checker (Academic Project – MSc Information Security & Digital Forensics)

📅 **Project Duration:** 25 November 2022 – 5 December 2022 (≈ 10 days, Part-Time)  
🎓 **Academic Year:** First Term (MSc Information Security & Digital Forensics)  
🏛️ **Institution:** University of East London, London, UK  
📘 **Subject:** Security Management  

📅 Project Context
This project was created as part of my MSc in Information Security and Digital Forensics
and later refined for portfolio purposes.

It is a Python-based tool that performs basic checks on small public websites to help
identify whether they appear to follow some visible aspects of GDPR best practice.

> Important: this tool is **not** a full legal assessment and does **not** replace
> professional legal or data protection advice. It is intended for learning,
> demonstration and initial technical checks only.

🏫 Project Overview

The GDPR Compliance Checker takes one or more website URLs and performs a series of
technical checks, including:

- Whether the site is served over HTTPS
- Whether a privacy policy or data protection page can be easily found
- Whether common cookie / consent scripts are present
- Basic inspection of HTTP headers (for example, security-related headers and cookies)
- Simple reporting to the console, CSV and/or Excel

The core logic is written in **Python**, using `requests` and `BeautifulSoup` for
HTTP and HTML parsing.

🎯 Project Objectives

- Practise analysing websites from a privacy and security perspective  
- Automate a set of repeatable checks for small websites  
- Produce simple, exportable reports for follow-up review  
- Use supporting tools (curl, Postman, SoapUI) to validate behaviour seen by the script  

🛠️ Core Technologies

- Python 3  
- `requests` for HTTP(S) requests  
- `BeautifulSoup` (bs4) for parsing HTML and searching for links / banners  
- `csv` / `pandas` or similar for simple reporting (CSV/Excel)  
- Command-line interface (CLI) for passing URLs and options  
- Manual verification with **curl**, **Postman** and **SoapUI** for selected sites  

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

📂 Project Structure (typical)

- `gdpr_checker.py` – main script or entry point  
- `helpers/` (optional) – helper modules for HTTP, parsing and reporting  
- `data/urls.txt` – example list of websites to scan  
- `reports/` – CSV or Excel outputs with summary results  
- `README.md` – project documentation (this file)  

🔍 What the Checker Looks For (Examples)

The exact checks may vary, but typical examples include:

- **Transport security**
  - Is the main URL accessible over `https://`?
  - Does the site redirect from `http://` to `https://`?
- **Privacy / data protection pages**
  - Can the script find links containing text such as “Privacy”, “Data Protection”,
    “Cookie Policy” or “GDPR”?
- **Cookie banners / consent tools**
  - Are there common CSS/JS patterns for consent tools (for example, banner IDs,
    classes or well-known script URLs)?
- **Headers and cookies (technical only)**
  - Are there obvious security-related headers present (e.g. `Strict-Transport-Security`,
    `Content-Security-Policy`, `X-Frame-Options`)?
  - Do `Set-Cookie` headers show flags such as `Secure` and `HttpOnly`?

The script records a simple “yes/no/unknown” style result for each check per site.
These can then be reviewed by a human who understands context and legal requirements.

## ▶️ Usage (Example)

Example: run checks for a small list of sites provided in `data/urls.txt`:

```bash
python gdpr_checker.py --input data/urls.txt --output reports/gdpr_results.csv
```

Possible command-line options (these may differ slightly in the actual implementation):

- `--input` – path to a text/CSV file of URLs  
- `--output` – path to CSV/Excel output file  
- `--timeout` – HTTP timeout in seconds  
- `--max-pages` – maximum number of pages to follow per site (if implemented)  

## 🌐 HTTP and API Testing (Postman / SoapUI)

Although the main tool is a Python script, I also used **curl**, **Postman** and
**SoapUI** to manually verify and explore how websites respond, especially when:

- Comparing behaviour seen by a browser versus raw HTTP requests  
- Inspecting redirects from `http://` to `https://`  
- Looking at full response headers and cookies for individual requests  
- Testing any JSON or XML endpoints (for example, public APIs or contact forms)

Typical manual steps included:

- Using **curl** or Postman to send `GET` and `HEAD` requests to:
  - the home page (e.g. `/`)
  - likely privacy URLs (e.g. `/privacy`, `/privacy-policy`, `/data-protection`)
- Using **Postman**’s interface to view response headers, cookies and redirects  
- Using **SoapUI** for experiments with XML-based or SOAP-style endpoints on sites
  that still expose legacy services

These manual checks helped validate and refine what the Python script was doing and
gave me a better feel for how different sites implement GDPR-related content.

## ⏱️ Project Timeline

| **Date Range** | **Task** |
|----------------|----------|
| 25 Nov 2022 | Requirement analysis and project planning |
| 26–28 Nov 2022 | Python module development |
| 29–30 Nov 2022 | Website scanning logic and regex patterns |
| 1–3 Dec 2022 | Report generation and compliance scoring |
| 4 Dec 2022 | Testing and debugging |
| 5 Dec 2022 | Final documentation and submission |

## ⚠️ Limitations

This project has several important limitations:

- It cannot determine whether a website is fully GDPR-compliant – it only checks a
  few visible technical and content indicators.
- Many aspects of GDPR are about organisational processes and legal wording that
  cannot be checked automatically.
- Some checks may produce false positives or miss content that is only available
  after certain user interactions (for example, cookie banners that load via JavaScript).

Because of this, the tool should be treated as:

- a **learning exercise**, and  
- a **first-pass technical checklist** for small websites, not a final audit.

---

## 📜 Disclaimer

This project is for educational and demonstration purposes only. It is not legal advice
and does not guarantee compliance with GDPR or any other regulation.

Anyone responsible for real-world compliance should seek appropriate legal and
data protection guidance.

---

## ✨ Author

Name: Anilkumar Dave  
Email: daveanil48@gmail.com
