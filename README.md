# 🌌 Planet Hunt - Asteroid Classification Challenge

A data science project for the Yuri’s Night "Planet Hunt" competition hosted by the IIT (BHU) Astronomy Club. This project dives deep into asteroid data from NASA JPL, aiming to analyze and classify asteroids based on their potential threat to Earth using machine learning techniques and statistical exploration.

---

## 📊 Project Objective

To assist the fictional data scientist **Samarth** in identifying potentially hazardous asteroids by analyzing:
- Orbital patterns
- Physical characteristics
- Classification flags (NEO, PHA)
  
We use **EDA**, **feature engineering**, and **classification models** to detect Near-Earth Objects, Potentially Hazardous Asteroids, and Main-Belt asteroids.

---

## 📁 Dataset

- Source: NASA JPL Asteroid Dataset  
- Format: `.csv`
- Fields include:  
  - `H` (Absolute Magnitude)  
  - `diameter`  
  - `albedo`  
  - `moid_ld` (Minimum Orbit Intersection Distance)  
  - `a` (Semi-Major Axis)  
  - `neo`, `pha` (classification flags)  
  - and more...

> The dataset used: `transformed_data (1).csv`  
> Problem statement: Included as `planet_hunt.pdf`

---

## 🧪 Tasks Performed

| Task | Description |
|------|-------------|
| ✅ Data Inspection | Datatypes, stats, missing values |
| ✅ EDA | Heatmap of detection methods, histograms |
| ✅ Feature Engineering | Created `moid_to_sma_ratio` |
| ✅ Class Imbalance Handling | Strategy: class weights in classifier |
| ✅ Skewness & IQR | Measured for `H`, `diameter`, `albedo` |
| ✅ Classification | Multiclass classifier for asteroid types |

---

## 📈 Results

- **Random Forest Classifier** achieved reasonable accuracy in classifying:
  - `0`: Main-belt asteroid
  - `1`: Near-Earth Object
  - `2`: Potentially Hazardous Asteroid (PHA)

- Confusion Matrix and classification report included in the notebook.

---

## 🧠 Model Info

- Model: `RandomForestClassifier` with class weights  
- Features used:
  - `H`, `diameter`, `albedo`, `moid_ld`, `a`, `moid_to_sma_ratio`

---

## 🚀 Run in Google Colab

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Upload the CSV dataset
3. Run all cells for full analysis

---

## 📌 How to Use

```bash
git clone https://github.com/your-username/planet-hunt-asteroid.git
cd planet-hunt-asteroid
