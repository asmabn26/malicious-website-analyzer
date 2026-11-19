# Malicious Website Analyzer

**Web-Based URL Security Analysis and Phishing Detection Tool**

## Overview

Malicious Website Analyzer is an academic cybersecurity project developed to help identify potentially malicious or fraudulent websites.

The application combines multiple security indicators to assess URL-related risks and provides a consolidated risk assessment through a web interface.

## Key Features

- **URL Reputation Analysis:** Integration with Google Safe Browsing to identify reported threats.
- **Phishing Indicators:** Detection of suspicious keywords and URL shortening services.
- **SSL/TLS Verification:** Inspection of HTTPS certificate information and security configuration.
- **DNS Analysis:** Examination of domain DNS records.
- **WHOIS Analysis:** Retrieval of domain registration information.
- **SQL Injection Indicators:** Identification of suspicious URL parameters and patterns.
- **XSS Indicators:** Detection of potentially dangerous URL patterns.
- **Risk Assessment:** Consolidation of findings into a website risk score.

**Important:** SQL injection and XSS checks are indicator-based. They do not constitute comprehensive vulnerability testing or exploitation.

## Project Demonstration

## Video Demo

A video demonstration of the **Malicious Website Analyzer** showcases the application's interface and URL security analysis workflow.

https://github.com/user-attachments/assets/92637ca8-f618-4c94-bf84-d5e764b022dc

The demonstration highlights the application's main functionalities, including:

- URL submission and security analysis.
- Detection of suspicious and potentially malicious URLs.
- Website reputation verification.
- SSL/TLS certificate inspection.
- DNS and WHOIS information analysis.
- Visualization of security findings and risk assessment results.

> **Disclaimer:** This tool is an academic cybersecurity project intended for educational and authorized security analysis. Its results should not be considered a definitive guarantee of website safety.








## Technologies Used

| Category | Technologies |
|---|---|
| Backend | Python, Flask |
| Frontend | HTML, CSS, JavaScript |
| API | Google Safe Browsing |
| Security Analysis | SSL/TLS, DNS, WHOIS |
| Python Libraries | Requests, BeautifulSoup, Cryptography, dnspython |
| Containerization | Docker (configuration included) |

## Project Structure

```text
malicious-website-analyzer/
├── app.py
├── requirements.txt
├── Dockerfile
├── .env.example
├── .gitignore
├── README.md
├── analyse.html
├── about.html
├── help.html
├── page.html
├── style.css
├── hover.js
├── Acceuil/
└── style/
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/malicious-website-analyzer.git
cd malicious-website-analyzer
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Create a virtual environment

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the API key

Copy `.env.example` to `.env` and configure your Google Safe Browsing API key.

```env
GOOGLE_SAFE_BROWSING_API_KEY=your_api_key_here
```

Never commit your actual API key.

### 5. Run the application

```bash
python app.py
```

Open the local address displayed by Flask, typically `http://127.0.0.1:5000`, and use the application's interface to submit a URL for analysis.

## Security Considerations

- The application is intended for educational and authorized security analysis.
- URL-based SQL injection and XSS indicators do not prove that a website is vulnerable.
- The absence of detected threats does not guarantee that a website is safe.
- API credentials must remain confidential.
- The Flask development server is not intended for production deployment.
- Public deployment requires additional security hardening.

## Future Improvements

- Automated unit and integration testing.
- Improved URL validation and protection against server-side request forgery (SSRF).
- CI/CD integration using GitHub Actions.
- Improved Docker deployment configuration.
- Historical scan reports and visualization.
- More advanced phishing detection techniques.

## Author

**Asma Bensassi Nour**

Cyberdefense Engineering Student — ENSA Marrakech

Academic cybersecurity project focused on web security analysis and malicious URL detection.
