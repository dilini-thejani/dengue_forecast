# Dengue Forecasting in Sri Lanka

This repository contains the implementation of a data-driven forecasting model for dengue incidence in Sri Lanka, leveraging climatic and epidemiological data. The project utilizes Random Forest Regressor and other statistical methods to analyze historical dengue trends and predict future outbreaks.

This work was carried out by Dilini Thejani Karunasena as part of a Master's in Industrial Mathematics at the University of Peradeniya, Sri Lanka, under the supervision of Dr. Lakshika S. Nawarathna.

---

## Overview

Dengue fever is a significant public health challenge in Sri Lanka. This project focuses on:
- Analyzing the relationship between dengue incidence and climatic factors (precipitation, temperature, humidity).
- Conducting spatial and temporal hotspot analyses.
- Building a Random Forest-based forecasting model to predict dengue trends for future years.

Key outputs include:
- Time-series visualizations of dengue incidence.
- Spatial hotspot analyses by province.
- Monthly risk analysis.
- Forecasts for dengue incidence in 2023 and 2024.

---

## Features

- **Data Visualization**: Explore the distribution of dengue cases over time and space.
- **Correlation Analysis**: Identify relationships between climatic factors and dengue incidence.
- **Machine Learning Model**: Predict future dengue outbreaks using Random Forest Regressor.
- **Interactive Use in Google Colab**: Easily run and adapt the code using Jupyter notebooks.

---

## Installation and Setup

### Prerequisites
- Google account for Google Colab
- Python libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

### Getting Started
1. **Clone the repository**:
   ```bash
   git clone https://github.com/dilini-thejani/dengue_forecast.git
   cd dengue_forecast
   ```
2. **Upload the repository files to Google Drive**:
   - Place the repository folder in your Google Drive.

3. **Run in Google Colab**:
   - Open the Jupyter notebook files (`*.ipynb`) in Google Colab.
   - Mount your Google Drive:
     ```python
     from google.colab import drive
     drive.mount('/content/drive')
     ```
   - Adjust file paths as needed to access the data files stored in Google Drive.

---

## Usage

1. **Prepare Data**:
   - Ensure all necessary data files (e.g., climate and dengue datasets) are stored in a Google Drive folder.
   - Update file paths in the notebooks to match your Google Drive structure.

2. **Run Analysis**:
   - Execute the notebook cells step-by-step in Google Colab.
   - Key analyses include:
     - Time series visualization
     - Hotspot analysis
     - Correlation tests
     - Model training, testing, and forecasting

3. **Interpret Results**:
   - Visualize outputs such as heatmaps, time-series plots, and forecast graphs.
   - Forecast dengue cases for specific years or provinces.

---

## Results

- **Accuracy Metrics (Western Province)**:
  - Mean Absolute Error (MAE): ~6966 cases.
  - R-Squared (R²): 76.22%.
- **Key Findings**:
  - Positive correlation between dengue incidence and precipitation/humidity.
  - High-risk provinces and months identified via hotspot analysis.

---

## Repository Structure

```plaintext
dengue_forecast/
├── Datasets/              # Main datasets (stored in Google Drive)
│   ├── Climate            # Monthly climate data (Precipitation, Humidity, Temperature) for each province from 2010 to 2022
│   ├── Dengue             # Monthly Dengue case data for each province from 2010 to 2022
├── Time Series Plots/     # Data files used for time series visualizations (used in time_series_plots.ipynb | stored in Google Drive)
├── Total Incidence/       # Annual total dengue cases for each province (used in prediction.ipynb | stored in Google Drive)
├── Independent Study-Final Report.pdf   # Comprehensive project documentation
├── README.md              # Project overview and documentation
├── heatmaps.ipynb         # Visualization of province-wise heatmap correlation between dengue incidence and climate factors
├── histograms.ipynb       # Frequency distribution of dengue incidence
├── shapiro_wilki_test.ipynb       # Statistical analysis (Shapiro-Wilk test)
└── time_series_plots.ipynb        # Time series visualization of annual dengue incidence and climate factors
```

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

---

## Acknowledgments

This research was supervised by **Dr. Lakshika S. Nawarathna** and supported by the Postgraduate Institute of Science, University of Peradeniya. Data was sourced from the Epidemiology Unit of the Ministry of Health and NASA's Data Access Viewer.

---
