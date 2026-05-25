# weather-history-eda
Exploratory Data Analysis (EDA) on historical weather data to validate core meteorological hypotheses and thermodynamic laws using Python.
# 🌤️ Weather Trends & Statistical Insights (EDA)

A data-driven Exploratory Data Analysis (EDA) project that tests real-world weather patterns, flags sensor issues, and reveals how temperature, pressure, and wind speed interact in nature.

---

## 🚀 Why This Project Matters
Instead of just plotting basic graphs, this project treats meteorological rules as data puzzles. By writing rigorous data pipelines in Python, I validated established weather theories using historical empirical data—making sure the dataset is structurally sound and ready for Machine Learning.

---

## 📊 3 Big Discoveries From the Data

### 1. Wind Speed vs. Visibility (The Air Clearing Effect)
* **What I Tested:** Does higher wind speed actually clear the air?
* **What the Data Showed:** Severe drops in visibility (< 1 km) happen **only** when wind speed is very low. The moment wind speed picks up, it creates turbulence that clears the air, and visibility stabilizes perfectly.

### 2. Barometric Pressure vs. Humidity (The Storm Warning)
* **What I Tested:** How does air pressure signal a coming storm?
* **What the Data Showed:** I found a strict natural boundary. Whenever atmospheric pressure drops below **1000 mb**, relative humidity automatically locks at its highest levels (**80%–100%**). This acts as a reliable data-driven alarm for incoming storms.

### 3. Rain vs. Snow (The Freezing Line)
* **What I Tested:** What exact conditions cause snow instead of rain?
* **What the Data Showed:** By analyzing temperature and humidity together, I mapped nature's exact boundary line:
  * **$0^\circ\text{C}$** is the absolute dividing line. Above this, it rains; below this, it snows.
  * Both rain and snow strictly require a high-humidity baseline of **$>80\%$** to actually fall.

---

## 🚨 Anomaly Detection: Catching a Sensor Glitch
Real-world data is never perfect. While analyzing the data, I caught a major hardware error that automated tools would miss:
* **The Error:** The dataset recorded a `Snow` event at exactly **`0.0%` Humidity**.
* **The Logic:** Physics dictates that snow cannot form or fall in a completely dry vacuum. I flagged this data point as a **sensor glitch**, demonstrating why human data cleaning is vital before building AI models.

---

## 🛠️ Tools & Tech Stack
* **Language:** Python 3
* **Data Wrangling:** `pandas` & `numpy`
* **Visualizations:** `seaborn` & `matplotlib` (Joint plots, threshold distribution matrices)

---
## Author
Tejal Joshi

## 📂 Quick Start
```bash
# Clone this repository
git clone [https://github.com/Tejaljoshi25-dotcom/weather-history-eda.git](https://github.com/Tejaljoshi25-dotcom/weather-history-eda.git)

# Open the notebook
# Launch 'Weather history (1).ipynb' in Jupyter or Google Colab to see the full code.


