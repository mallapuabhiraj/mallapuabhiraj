# Abhi Raju Mallapu

**Machine Learning Engineer · Embedded Systems Developer · Software Engineer**

> *"I build systems that think, react, and perform — whether in silicon or in code."*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/abhirajmallapu)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mallapuabhiraj)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:abhirajmallapu@gmail.com)

---

## Who Am I

B.Tech (EEE) student at Sri Venkateswara University College of Engineering, Tirupati — operating at the intersection of **Machine Learning**, **Software Engineering**, and **Embedded Systems**.

I don't just train models or flash firmware. I build **complete, production-minded solutions** — from 1M-row ML pipelines backed by industry cost research, to IoT greenhouse controllers that learned about flyback diodes the expensive way.

- 🧠 ML pipelines built around **business-first metrics** — PR-AUC, cost-sensitive thresholds, out-of-time generalization
- ⚙️ Embedded firmware built on **real hardware failures** — three-layer signal filtering, watchdog protection, crash-proof control loops
- 🔗 Comfortable bridging **data intelligence** and **physical systems** — a rare and practical combination
- 🚀 Actively seeking roles in **ML Engineering**, **SDE**, **Embedded Systems**, and **SDE-Embedded**

---

## 🛠️ Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![C++](https://img.shields.io/badge/Embedded%20C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)

**Machine Learning & Data Science**

![CatBoost](https://img.shields.io/badge/CatBoost-FFCC00?style=for-the-badge&logoColor=black)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=for-the-badge&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=for-the-badge&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Optuna](https://img.shields.io/badge/Optuna-3B4EFF?style=for-the-badge&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-FF4B4B?style=for-the-badge&logoColor=white)

**Production & Engineering**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

**Embedded & Hardware**

![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Blynk](https://img.shields.io/badge/Blynk-00C878?style=for-the-badge&logoColor=white)
![ThingSpeak](https://img.shields.io/badge/ThingSpeak-0076A8?style=for-the-badge&logoColor=white)
![VS Code](https://img.shields.io/badge/VSCode-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 🚀 Projects

> *Recruiters who read this far get a free mental high-five. Here's what I've actually built:*

---

### 🌱 TerraFirm — ESP32 Greenhouse Monitoring & Control

![Platform](https://img.shields.io/badge/ESP32-Firmware-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Signal](https://img.shields.io/badge/Signal%20Pipeline-3%20Layers-brightgreen?style=flat-square)
![Cloud](https://img.shields.io/badge/Cloud-Blynk%20%2B%20ThingSpeak-blue?style=flat-square)

> *ESP32 · Arduino C++ · DHT11 · Capacitive Soil Sensor · Blynk · ThingSpeak · I2C LCD*

**[→ terrafirm](https://github.com/mallapuabhiraj/terrafirm)**

Automated greenhouse firmware that manages watering and ventilation in real time — built through actual hardware failures and a deeply personal relationship with the IN4007 diode.

- 🔬 **Three-layer signal pipeline** — median filter → EMA smoothing → 30s circular buffer. Raw ADC jumping 0%→97%→12%? After filtering: 42%→43%→43%. Pump correctly idle
- 🛡️ **9-layer safety system** — boot-pulse suppression, 30s pump timeout, 60s cooldown, DHT fault tolerance (5-failure threshold), hardware watchdog, exponential WiFi backoff
- 📡 **Dual cloud + offline capable** — Blynk for live remote control, ThingSpeak for trend logging; full local control + LCD continues with zero WiFi
- 💀 **Built through real failures** — unregulated li-ion batteries crashing USB bridges, relay flyback spikes freezing Serial Monitor, raw ADC hallucinating moisture readings. Every safety layer is a failure that happened
- ⚡ **Crash-proof loop** — non-blocking `loop()`, hardware watchdog on 10s timeout, exponential WiFi backoff preventing reconnect spam from starving the control cycle

---

### 🕵️ Credit Card Fraud Detection + Production API

![PR-AUC](https://img.shields.io/badge/PR--AUC-0.9284-brightgreen?style=flat-square)
![Tests](https://img.shields.io/badge/Tests-17%20Passing-brightgreen?style=flat-square)
![CI](https://github.com/mallapuabhiraj/fraud-detection-catboost/actions/workflows/tests.yml/badge.svg)

> *Python · CatBoost · FastAPI · PostgreSQL · SQLAlchemy · Optuna · pytest · GitHub Actions*

**[→ fraud-detection-catboost](https://github.com/mallapuabhiraj/fraud-detection-catboost)**

Finding fraud in a dataset where 994 out of every 1000 transactions are legitimate. Standard accuracy? Useless. This project optimizes for what actually matters.

- 🧠 Engineered **40+ domain-driven features** — geospatial anomaly detection, temporal behavioral aggregation, impossible travel detection, dormant card reactivation
- 🔒 **Leakage-safe chronological validation** — no peeking at the future, ever
- ⚙️ Replaced XGBoost (0.67 PR-AUC, 0.11 val→test gap) with CatBoost's native ordered encoding → **0.93 PR-AUC, 0.028 gap**
- 💰 Threshold tuned to **0.830** using real industry cost data — LexisNexis True Cost of Fraud 2024, Ravelin, MIT LIDS, Chargeflow — not assumptions
- 🌍 **Out-of-time drift test**: base model collapsed at 2.2% fraud rate (0.6471 PR-AUC) → retrained model held at **0.9997 PR-AUC** (+35.26%)
- 🌐 Served via **FastAPI** with 4 endpoints, PostgreSQL prediction logging, 17 pytest tests, and CI/CD via GitHub Actions

---

### 🎣 PhreshCatch — Phishing URL Detection

![ROC-AUC](https://img.shields.io/badge/ROC--AUC-0.9804-brightgreen?style=flat-square)
![Catch Rate](https://img.shields.io/badge/Phishing%20Catch%20Rate-97.74%25-brightgreen?style=flat-square)

> *Python · XGBoost · LightGBM · Optuna · SHAP · PhreshPhish*

**[→ phreshcatch](https://github.com/mallapuabhiraj/phreshcatch)**

Classifying URLs as phishing or benign using **nothing but the URL string itself**. No page visits. No DNS lookups. No HTML parsing. Just 27 features and 0.4ms to decide.

- 🔍 **Caught two dataset construction flaws** before a single model was trained — a leaking feature scoring 100.0 on every legitimate URL, and HTML features reflecting scraping completeness, not malice
- 🌍 **Cross-dataset generalization test**: 99% accuracy on PhiUSIIL → **23% phishing recall** on ISCX. Same model. Complete collapse. Documented why, switched to PhreshPhish
- 🧠 **PathLength** emerged as the #1 SHAP feature — not in the original feature set, discovered during engineering. Restructured the entire importance hierarchy
- 🎯 Threshold tuned to **0.57**: saves 628 phishing URLs vs default, at a 1:1.3 FP tradeoff. Annoyed users recover. Compromised accounts don't
- ✅ **97.74% catch rate** on 168K test URLs — stress tested across 6 attack categories with honest failure breakdown (7 misses, root causes documented)

---

### 🫀 Heart Disease Prediction

![Recall](https://img.shields.io/badge/Recall-90.9%25-brightgreen?style=flat-square)
![Accuracy](https://img.shields.io/badge/Accuracy-86.9%25-brightgreen?style=flat-square)
![Colab](https://colab.research.google.com/assets/colab-badge.svg)

> *Python · Scikit-Learn · SVM · GridSearchCV · Optuna · Pipeline · Feature Engineering*

**[→ heart-disease-prediction](https://github.com/mallapuabhiraj/heart-disease-prediction)**

Predicting cardiovascular disease from 13 routine clinical features — optimizing specifically for recall, because a false negative here isn't a bad metric. It's a person.

- 🔬 Engineered **10 clinically motivated features** on top of the original 13 — `severity_score`, `high_risk_profile`, `hr_ratio`, `exercise_risk` — encapsulated in a reusable sklearn `TransformerMixin`
- 🏆 **2 of the top 3 predictors were engineered features** — independently confirmed by both LR and RF importance rankings
- ⚖️ Threshold swept across the precision-recall curve to find the **highest threshold still achieving ≥90% recall** — tuning beat model selection entirely; all three models hit identical recall after this step
- 🥇 **SVM won the tiebreaker** — fewest false positives (5 vs 8 vs 9), highest accuracy (86.9%), highest F1 (0.882) — fewer healthy patients wrongly alarmed
- 🔒 End-to-end **sklearn Pipelines** (`Preprocess → StandardScaler → Model`) — zero data leakage guaranteed across every cross-validation fold

---

### 🔥 Gas Leakage Detection & Protection System

> *Arduino C++ · Arduino Uno · MQ-135 · Servo Motor · Buzzer · LED*

Real-time embedded safety system that detects hazardous gas leaks and autonomously triggers protective responses — modeled after industrial substation safety standards.

- 🧪 MQ-135 sensor with precision threshold calibration for reliable, low-false-alarm hazard detection
- ⚡ **Sub-2-second response** within 100cm — simultaneous buzzer alert, servo-driven gas valve closure, LED status indication
- 🏭 Architected to mirror real-world substation safety protocols — production-aware embedded systems thinking

---

### ☀️ Single-Axis Solar Tracker

> *Arduino C++ · Arduino Uno · LDR Sensors · Servo Motor · Solar Panel*

Closed-loop embedded control system that autonomously tracks sunlight across a full arc to maximize solar energy yield.

- 📡 Dual LDR differential sensing driving a real-time precision control loop across 180° sunlight arc
- ⚡ **25–40% higher energy capture** and **20–30% daily power boost** over static panel installations
- 🔧 Demonstrates closed-loop control, sensor integration, PWM servo positioning, and firmware optimization

---

## 🏆 Leadership

**Event Coordinator — E-BLAZE 2K25**, SVUCE Tirupati
Directed end-to-end logistics for **300+ attendees** across colleges in Andhra Pradesh — registrations, multi-track scheduling, on-ground operations. Ownership, coordination under pressure, large-scale execution.

---

## 💼 Open To

![ML Engineering](https://img.shields.io/badge/ML%20Engineering-FF6F00?style=for-the-badge&logoColor=white)
![Software Engineering](https://img.shields.io/badge/Software%20Engineering-0078D4?style=for-the-badge&logoColor=white)
![Embedded Systems](https://img.shields.io/badge/Embedded%20Systems-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![SDE Embedded](https://img.shields.io/badge/SDE%20Embedded-6A0DAD?style=for-the-badge&logoColor=white)

---

*⚡ Recall over accuracy. Real-world impact over benchmark glory. ⚡*
