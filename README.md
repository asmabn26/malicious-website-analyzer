# Malicious Website Analyzer

Outil web d'analyse de risque d'URL développé dans le cadre d'un projet académique de cybersécurité. Il regroupe plusieurs signaux techniques afin d'aider à repérer des sites potentiellement malveillants ou frauduleux.

> Projet académique. Les résultats sont indicatifs et ne remplacent pas une analyse de sécurité professionnelle.

## Analyse effectuée

- Réputation d'URL avec Google Safe Browsing.
- Indices de phishing : mots-clés sensibles et raccourcisseurs d'URL.
- Configuration SSL/TLS et certificats.
- Informations DNS et WHOIS.
- Paramètres URL suspects associés aux risques d'injection SQL et XSS.
- Score de risque consolidé dans une interface web.

## Technologies

Python 3 · Flask · Flask-CORS · Requests · BeautifulSoup · DNS/WHOIS · Cryptography · HTML/CSS/JavaScript

## Installation

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
Copy-Item .env.example .env
python app.py
```

Ajoutez votre propre clé API dans `.env`, puis ouvrez l'adresse affichée par Flask (généralement `http://127.0.0.1:5000`).

## Sécurité et limites

- Ne publiez jamais `.env` ni une clé API.
- Utilisez l'outil uniquement sur des URL dont l'analyse est autorisée.
- Une absence d'alerte ne garantit pas qu'un site est sûr.

## Auteur

Asma Bensassi Nour — Étudiante ingénieure en Cyberdéfense, ENSA Marrakech.
