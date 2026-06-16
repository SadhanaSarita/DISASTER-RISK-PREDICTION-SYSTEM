🏔️ Uttarakhand Disaster Prediction & Warning System

An end-to-end AI-powered disaster risk prediction and early warning system for Uttarakhand, India — built using NASA POWER satellite data and Random Forest Machine Learning.

Overview
Uttarakhand is one of India's most disaster-prone states, experiencing devastating floods, landslides, forest fires, and heat waves every year. This system predicts disaster risk before it happens by analysing satellite weather data using machine learning — giving early warnings to help save lives.
Validated against the Kedarnath 2013 tragedy — the system was backtested on June 2013 NASA data to check if it would have issued an early warning before one of India's worst natural disasters (5,700+ lives lost).

🎯 What It Does
Predicts 4 disaster types simultaneously — Forest Fire, Flood, Landslide, Heat Wave
Covers the entire Uttarakhand region on a 9×9 spatial grid
Generates daily risk scores for every grid cell (50×70 km resolution)
Issues colour-coded alerts — 🟢 Green / 🟡 Yellow / 🟠 Orange / 🔴 Red
Displays results on an interactive map and dashboard

📊 Data Sources
1. NASA POWER MERRA-2 (Primary)
Satellite-derived meteorological data downloaded via NASA POWER API.
Region: LAT 28°N – 32°N | LON 77°E – 81°E (Uttarakhand)
Period: March 2025 – March 2026
Grid: 9 × 9 spatial grid (81 cells)
Total Records: 24,156 rows

2. SDMA Alert Details
35 official disaster alerts from the State Disaster Management Authority and Forest Survey of India.

3. IMD Nowcast Alerts
141 short-term weather alerts from the India Meteorological Department.

Districts Covered
Dehradun · Haridwar · Pauri · Tehri · Uttarkashi · Chamoli · Rudraprayag · Nainital · Almora · Bageshwar · Pithoragarh · Champawat

Kedarnath 2013 Validation
Event: June 16–17, 2013 — Kedarnath cloudburst and flash floods — 5,700+ deaths
Test: Downloaded NASA POWER data for June 2013, ran trained ML models on pre-disaster days, checked if RED alert would have been issued before June 16.
Grid Cell: Nearest to Kedarnath (30.7°N, 79.0°E)
This backtest demonstrates the system's ability to detect dangerous conditions using only satellite weather data — without any ground sensor input.

📚References
NASA POWER Project: power.larc.nasa.gov
MERRA-2 Reanalysis: Gelaro et al., 2017, Journal of Climate
IMD Disaster Guidelines: India Meteorological Department
NDMA Uttarakhand: National Disaster Management Authority
Kedarnath 2013: NDMA Post-Disaster Needs Assessment Report
This project is for academic and research purposes.
Data sourced from NASA POWER (public domain) and IMD/SDMA (government open data).
