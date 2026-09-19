# 🧪 QA Automation Portfolio: WeatherAPI Testing & Dynamic Date Automation

> About this repository: This project demonstrates automated API testing using Postman and JavaScript scripts for WeatherAPI services. It showcases advanced Postman capabilities, including dynamic date generation via the `moment.js` library in pre-request scripts, current weather checks, 3-day forecasting, and historical data retrieval. It also highlights a modern "Shift-Left" QA approach and Continuous Integration (CI/CD) readiness via Newman.

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Newman](https://img.shields.io/badge/Newman-026E42?style=for-the-badge&logo=postman&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

## 🎯 Project Overview

This collection provides automated API test scripts targeting WeatherAPI endpoints (`https://api.weatherapi.com` or custom base URLs). It validates real-time weather conditions, forecasts, and historical meteorological data archives.

As a QA Automation / API Testing Engineer, my focus in this repository is to implement dynamic runtime variable handling, leverage pre-request scripting for date calculations (e.g., automated past date formatting), and ensure reliable REST API contract validation across different timeframes.

## 🛠️ QA Tech Stack & Tools

* **API Testing Tool:** Postman
* **CLI Runner / CI Execution:** Newman
* **Scripting & Libraries:** JavaScript, Moment.js (Pre-request automation)
* **CI/CD Pipeline Support:** GitHub Actions
* **Target Environment:** WeatherAPI REST Services

## 📊 Test Strategy & Coverage

### 1. Automated API Testing & Endpoints
The Postman collection includes structured requests validating:
* **Current Day Weather (`GET /current.json`):** Fetches real-time weather data for specified locations (e.g., Warsaw).
* **Forecast for 3 Days (`GET /forecast.json`):** Validates multi-day meteorological forecasting capabilities.
* **Historical Weather Tracking (`GET /history.json`):** Tests past weather data retrieval across specific dates (beginning of the week, beginning of the month, and custom historical timestamps).

### 2. Advanced Pre-Request Automation
* **Dynamic Date Generation:** Utilizes a pre-request script with `moment.js` to automatically calculate and assign collection variables (`Yesterday`, `month_ago`, `start_of_week`, `start_of_month`), eliminating hardcoded date dependencies in historical test runs.

## 🚀 How to Run the Tests Locally

To run and evaluate this Postman collection locally using Node.js and Newman, follow these steps:

### 1. Prerequisites
Ensure you have Node.js installed, then install Newman globally (if not already installed):
```bash
npm install -g newman
