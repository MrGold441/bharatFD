
# BharatFD Backend Assignment

This repository contains the backend solution for the BharatFD assignment. The code is built as per the provided instructions and is available in the `main` branch.

# Table of Contents
1. [🌟 Features Implemented](#features-implemented)
2. [⚙️ Quick Setup without Docker](#quick-setup-without-docker)
3. [🐳 Quick Setup with Docker](#quick-setup-with-docker)
4. [📡 API Usage](#api-usage)
5. [🧩 Schema](#schema)
6. [💬 Contribution Guidelines](#contribution-guidelines)


## 🌟 Features Implemented:

- ✅ Automatic Translations while FAQ creation
- ✅ Optimized SQL queries with `Prefetch`
- ✅ Optimal Schema for production ready environment
- ✅ Multi-language translation using Google Translate
- ✅ REST API with language selection
- ✅ Individual FAQ translation and caching
- ✅ Redis caching for improved performance
- ✅ Unit tests for models and API

## ⚙️ Quick Setup (Without Docker 🐳)

To set up the project, install dependencies, and run the application, execute the following commands:

```bash
git clone  https://github.com/MrGold441/bharatFD.git
cd bharatFD
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py runserver
```

To run tests, use:

```bash
source venv/bin/activate
pytest
```

## ⚙️ Quick Setup (With Docker 🐳)

To set up the project with Docker, you can use the following command:

```bash
git clone  https://github.com/MrGold441/bharatFD.git
cd bharatFD
docker compose up --build
```

This will build the Docker image and run the application in the container, exposing the app on `http://localhost:80`. 


## 📡 API Usage
- For Localhost
```bash
# Fetch FAQs in English (default)
curl http://localhost:8000/api/faqs/

# Fetch FAQs in Hindi
curl http://localhost:8000/api/faqs/?lang=hi

# Fetch FAQs in Bengali
curl http://localhost:8000/api/faqs/?lang=bn
```
