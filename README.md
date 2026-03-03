# 🛰️ National Air & Sea Radar: Real-Time Surveillance Dashboard

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-Deployed-FF4B4B.svg)
![APIs](https://img.shields.io/badge/Data-WebSockets%20%7C%20REST-green.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)

## 📌 Overview
A real-time situational awareness dashboard tracking commercial airspace and maritime vessels around the Indian subcontinent. Built using Python and Streamlit, this application ingests live telemetry data via REST APIs and WebSockets, rendering it on an interactive geospatial map. 

This project demonstrates the ability to handle live, asynchronous data streams and deploy interactive web applications, expanding on previous work with Python-based Streamlit applications like predictive ML models and data analysis tools.

**Live Demo:** [Insert your deployed Streamlit URL here]

## 🚀 Features
* **Live Aviation Tracking:** Fetches real-time flight telemetry (coordinates, callsigns, country of origin) via the AirLabs REST API.
* **Live Maritime Tracking:** Establishes a WebSocket connection to `aisstream.io` to ingest continuous AIS (Automatic Identification System) vessel position reports.
* **Interactive Mapping:** Utilizes `folium` and `streamlit-folium` for high-performance geospatial data visualization.
* **Dynamic Filtering:** Automatically differentiates domestic vs. foreign-registered aircraft and plots active vessels within the specified bounding box.
* **Secure Credential Management:** Engineered to securely handle API keys using Streamlit Secrets for safe public deployment.

## 🛠️ Technology Stack
* **Language:** Python
* **Frontend/UI:** Streamlit
* **Geospatial Visualization:** Folium
* **Data Ingestion:** `requests` (REST), `websocket-client` (WSS)
* **Development Environment:** Google Colab / Local IDE

## 🛡️ Cybersecurity & Future Scope
Working with unencrypted public radio frequencies (AIS) presents unique data validation challenges. Future iterations of this project aim to incorporate:
* **Anomaly Detection:** Using Machine Learning to flag vessels that suddenly disable their AIS transponders or deviate from standard shipping lanes.
* **Signal Integrity:** Exploring concepts around detecting spoofed AIS/ADS-B signals.

## 💻 Local Setup & Installation

1. Clone the repository:
   ```bash
   git clone [https://github.com/Ullas33/National-Air-Sea-Radar.git]
   cd national-air-sea-radar
