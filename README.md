<div align="center">

<!-- Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=🌾%20AgriNexus&fontSize=72&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=AI-Powered%20Smart%20Farming%20Intelligence%20Platform&descAlignY=60&descAlign=50" width="100%"/>

<br/>

<!-- Badges -->
[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-2.x-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Heroku](https://img.shields.io/badge/Heroku-Deployed-430098?style=for-the-badge&logo=heroku&logoColor=white)](https://heroku.com)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![License](https://img.shields.io/badge/License-MIT-2ECC71?style=for-the-badge)](LICENSE)

<br/>

> **Empowering farmers with data-driven decisions** — AgriNexus combines machine learning with agricultural science to deliver precise crop and fertilizer recommendations, turning complex soil & climate data into actionable farming insights.

<br/>

---

</div>

## 📑 Table of Contents

- [✨ Overview](#-overview)
- [🚀 Key Features](#-key-features)
- [🧠 How It Works](#-how-it-works)
- [🛠️ Tech Stack](#️-tech-stack)
- [📁 Project Structure](#-project-structure)
- [⚙️ Installation & Setup](#️-installation--setup)
- [🌐 Deployment](#-deployment)
- [📊 ML Models](#-ml-models)
- [📸 Screenshots](#-screenshots)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Overview

**AgriNexus** is an end-to-end AI-powered agricultural intelligence platform designed to bridge the gap between modern machine learning and everyday farming practices. By analyzing soil composition, climate conditions, and environmental parameters, AgriNexus provides:

- 🌱 **Smart Crop Recommendations** — Know exactly which crop will thrive in your field
- 💊 **Precision Fertilizer Guidance** — Get tailored fertilizer suggestions to maximize yield
- 📈 **Data-Driven Insights** — Make informed decisions backed by real agricultural datasets

Whether you're a smallholder farmer or an agricultural researcher, AgriNexus brings the power of AI to your fingertips through a clean, intuitive web interface.

---

## 🚀 Key Features

| Feature | Description |
|---|---|
| 🌾 **Crop Recommendation** | Predicts the most suitable crop based on N, P, K values, temperature, humidity, pH, and rainfall |
| 🧪 **Fertilizer Recommendation** | Suggests optimal fertilizers based on soil nutrient deficiencies and crop type |
| 🌐 **Web Interface** | Clean, responsive Flask web app accessible from any device |
| 📓 **Jupyter Notebooks** | Full ML pipeline notebooks for transparency and reproducibility |
| ☁️ **Cloud Ready** | Deployed on Heroku with a Procfile-based configuration |
| 📦 **Modular Architecture** | Organized codebase with separate modules for models, utils, and configs |

---

## 🧠 How It Works

```
       Input Parameters
    ┌──────────────────────┐
    │  N · P · K · pH      │
    │  Temperature         │
    │  Humidity · Rainfall │
    │  Crop Type (optional)│
    └──────────┬───────────┘
               │
               ▼
    ┌──────────────────────┐
    │   Flask Web Server   │
    │     (app.py)         │
    └──────────┬───────────┘
               │
       ┌───────┴────────┐
       ▼                ▼
┌─────────────┐  ┌─────────────┐
│    Crop     │  │ Fertilizer  │
│ Recommender │  │ Recommender │
│    Model    │  │    Model    │
└──────┬──────┘  └──────┬──────┘
       └────────┬────────┘
                ▼
     ┌─────────────────────┐
     │   Recommendation    │
     │   & Actionable      │
     │     Insights        │
     └─────────────────────┘
```

The system processes 7 key agricultural parameters through trained ML models to generate recommendations in real-time.

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology |
|---|---|
| **Backend** | Python 3.8+, Flask |
| **ML / Data Science** | Scikit-learn, Pandas, NumPy |
| **Frontend** | HTML5, CSS3, JavaScript |
| **Notebooks** | Jupyter Notebook |
| **Deployment** | Heroku (Procfile + Gunicorn) |
| **Data** | Custom curated CSV datasets |

</div>

---

## 📁 Project Structure

```
AgriNexus/
│
├── 📂 AgriNexus/                    # Core application package
│
├── 📂 Data/                         # Processed datasets
├── 📂 Data-raw/                     # Raw / original source data
│
├── 📂 models/                       # Trained ML model files (.pkl)
│
├── 📂 static/                       # CSS, JS, images
│   ├── css/
│   └── js/
│
├── 📂 templates/                    # Jinja2 HTML templates
│   ├── index.html
│   └── result.html
│
├── 📂 utils/                        # Helper functions & utilities
│
├── 📓 Crop_data_preparation.ipynb              # Data prep notebook
├── 📓 Fertilizer_Recommendation_Model.ipynb    # Fertilizer ML notebook
├── 📓 Final_recommendationdata_creation.ipynb  # Final dataset creation
│
├── 📊 cpdata.csv                              # Crop prediction dataset
├── 📊 Fertilizer Prediction.csv               # Fertilizer raw data
├── 📊 Fertilizer_Recommendation.csv           # Fertilizer processed data
│
├── 🐍 app.py                        # Main Flask application entry point
├── ⚙️ config.py                     # Application configuration
├── 📋 requirements.txt              # Python dependencies
├── 🚀 Procfile                      # Heroku deployment config
└── 📄 README.md
```

---

## ⚙️ Installation & Setup

### Prerequisites

- Python 3.8 or higher
- pip package manager
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/akash4550/AgriNexus.git
cd AgriNexus
```

### 2. Create a Virtual Environment (Recommended)

```bash
# Create virtual environment
python -m venv venv

# Activate — macOS/Linux
source venv/bin/activate

# Activate — Windows
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
python app.py
```

### 5. Open in Browser

Navigate to: **[http://localhost:5000](http://localhost:5000)**

---

## 🌐 Deployment

AgriNexus is configured for deployment on **Heroku** out of the box.

```bash
# Login to Heroku
heroku login

# Create a new Heroku app
heroku create your-agrinexus-app

# Push to Heroku
git push heroku main

# Open the deployed app
heroku open
```

The `Procfile` handles the web dyno configuration automatically using Gunicorn.

---

## 📊 ML Models

### 🌾 Crop Recommendation Model

The crop recommendation engine is trained on agricultural data encompassing:

| Input Feature | Description |
|---|---|
| **N** | Nitrogen content in soil (kg/ha) |
| **P** | Phosphorus content in soil (kg/ha) |
| **K** | Potassium content in soil (kg/ha) |
| **Temperature** | Average temperature (°C) |
| **Humidity** | Relative humidity (%) |
| **pH** | Soil pH level |
| **Rainfall** | Annual rainfall (mm) |

**Output:** The crop best suited for the given conditions (e.g., Rice, Wheat, Maize, etc.)

### 🧪 Fertilizer Recommendation Model

The fertilizer recommender takes into account:
- Soil nutrient levels (N, P, K)
- Crop type
- Soil type

**Output:** The most appropriate fertilizer (e.g., Urea, DAP, 14-35-14, etc.)

### 📓 Notebooks

| Notebook | Purpose |
|---|---|
| `Crop_data_preparation.ipynb` | Data cleaning, preprocessing, and feature engineering for crop data |
| `Fertilizer_Recommendation_Model.ipynb` | Training and evaluation of the fertilizer recommendation model |
| `Final_recommendationdata_creation.ipynb` | Final dataset preparation pipeline |

---



## 🤝 Contributing

Contributions are welcome! Here's how you can help improve AgriNexus:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/AmazingFeature`
3. **Commit** your changes: `git commit -m 'Add some AmazingFeature'`
4. **Push** to the branch: `git push origin feature/AmazingFeature`
5. **Open** a Pull Request

### 🐛 Found a Bug?

Open an issue [here](https://github.com/akash4550/AgriNexus/issues) with a clear description and reproduction steps.

---

## 🌟 Future Roadmap

- [ ] 🌦️ Live weather API integration for real-time climate data
- [ ] 🗺️ Geo-location based recommendations
- [ ] 📱 Mobile-responsive progressive web app (PWA)
- [ ] 🔬 Soil image analysis using computer vision
- [ ] 📊 Yield prediction module
- [ ] 🌍 Multi-language support for regional farmers
- [ ] 🔔 SMS/WhatsApp alerts for crop advisory

---



<div align="center">

**Made with ❤️ for farmers everywhere**

[![GitHub](https://img.shields.io/badge/GitHub-akash4550-181717?style=for-the-badge&logo=github)](https://github.com/akash4550)

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>

</div>

