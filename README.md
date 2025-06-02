# Delhivery Feature Engineering Case Study

## 🚚 Project Overview
Delhivery is India’s largest, fully integrated logistics provider. Their mission is to build the commerce operating system through top-tier infrastructure, high-quality logistics operations, and advanced engineering and technology capabilities. The Data team at Delhivery leverages data to enhance operational efficiency, ensure data integrity, and support accurate forecasting models.

This repository contains a step-by-step implementation of the Delhivery Feature Engineering case study. All code cells, explanations, and visualizations have been refactored to follow Delhivery’s official “Feature Engineering – Solution Approach” document, ensuring clarity, completeness, and originality.

---

## 📂 Dataset
The CSV file contains trip- and segment-level information, including timestamps, distances, and OSRM routing estimates.  

- **Download URL:**  
https://d2beiqkhq929f0.cloudfront.net/public_assets/assets/000/001/551/original/delhivery_data.csv?1642751181


### Key Columns (After Dropping Irrelevant Fields)
- `trip_uuid`  
- `trip_creation_time`, `od_start_time`, `od_end_time` (timestamps)  
- `route_type` (FTL, Carting)  
- `source_center`, `source_name`  
- `destination_center`, `destination_name`  
- `actual_distance_to_destination`  
- `segment_actual_time`, `segment_osrm_time`, `segment_osrm_distance`  

---

## 🚀 How to Run (Google Colab)
1. **Open Colab:**  
 https://colab.research.google.com  

2. **Load the CSV directly:**
 ```python
 import pandas as pd

 url = "https://d2beiqkhq929f0.cloudfront.net/public_assets/assets/000/001/551/original/delhivery_data.csv?1642751181"
 df = pd.read_csv(url)
 df.head()
