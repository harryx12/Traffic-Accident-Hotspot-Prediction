# Traffic Accident Hotspot Prediction

A machine learning project for predicting traffic accident hotspots using historical accident data, feature engineering, geospatial analysis, developed in June 2023.

---

## Project Overview

This notebook builds an end-to-end pipeline for:

* Downloading and loading traffic accident datasets
* Cleaning and preprocessing accident records
* Engineering meaningful spatial and temporal features
* Performing exploratory data analysis (EDA)
* Training machine learning models for hotspot prediction
* Evaluating model performance and optimizing thresholds
* Explaining predictions using SHAP values
* Visualizing accident hotspots on an interactive map
* Saving trained models and artifacts for inference

The project uses ensemble-based machine learning models such as:

* XGBoost
* LightGBM
* Scikit-learn models

It also includes:

* Interactive hotspot visualization with Folium
* Explainability with SHAP
* Imbalanced data handling with imbalanced-learn

---

## Features

### Data Processing

* Missing value handling
* Feature encoding
* Numerical scaling
* Temporal feature extraction
* Spatial feature engineering

### Exploratory Data Analysis

* Accident distribution analysis
* Correlation analysis
* Temporal trend visualization
* Geographic hotspot exploration

### Machine Learning

* Preprocessing pipeline
* Model training and validation
* Threshold tuning
* Performance evaluation
* Feature importance analysis

### Explainability

* SHAP explainability visualizations
* Feature importance ranking
* Model interpretation

### Visualization

* Interactive Folium hotspot maps
* Plotly visualizations
* Matplotlib and Seaborn charts

---

## Technologies Used

### Programming Language

* Python 3.x

### Libraries

* pandas
* numpy
* scikit-learn
* xgboost
* lightgbm
* imbalanced-learn
* shap
* folium
* matplotlib
* seaborn
* plotly
* joblib

---

## Project Structure

```text
Traffic_Accident_Hotspot_Prediction.ipynb
│
├── Install & Import Dependencies
├── Kaggle Authentication & Dataset Download
├── Data Loading & Initial Inspection
├── Feature Engineering & Preprocessing
├── Exploratory Data Analysis (EDA)
├── Build Preprocessing Pipeline
├── Model Training
├── Evaluation & Threshold Tuning
├── Feature Importance & SHAP Explainability
├── Interactive Hotspot Map (Folium)
├── Save Models & Artifacts
└── Inference: Predict on New Data
```

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/traffic-accident-hotspot-prediction.git
cd traffic-accident-hotspot-prediction
```

### Create a Virtual Environment (Optional)

```bash
python -m venv venv
```

Activate the environment:

#### Windows

```bash
venv\Scripts\activate
```

#### macOS/Linux

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install pandas numpy scikit-learn xgboost lightgbm imbalanced-learn shap folium matplotlib seaborn plotly joblib
```

---

## Dataset

The notebook downloads accident-related datasets using Kaggle.

### Kaggle Setup

1. Create a Kaggle account
2. Generate a Kaggle API token
3. Place `kaggle.json` inside:

```text
~/.kaggle/
```

Or for Windows:

```text
C:\Users\<USERNAME>\.kaggle\
```

---

## Workflow

### 1. Data Loading

The dataset is loaded into pandas DataFrames and inspected for:

* Missing values
* Data types
* Duplicate records
* Statistical summaries

### 2. Feature Engineering

Features are created from:

* Date and time columns
* Geographic coordinates
* Accident severity information
* Environmental and contextual data

### 3. Exploratory Data Analysis

EDA helps identify:

* Accident trends
* Peak accident times
* High-risk locations
* Important predictive variables

### 4. Model Training

The notebook trains machine learning models using preprocessing pipelines and evaluates them using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC

### 5. Threshold Optimization

Prediction thresholds are tuned to improve hotspot classification performance.

### 6. Explainability

SHAP is used to explain:

* Global feature importance
* Individual predictions
* Model behavior

### 7. Interactive Mapping

Folium maps visualize:

* Accident clusters
* Predicted hotspots
* Geographic accident intensity

---

## Running the Notebook

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
Traffic_Accident_Hotspot_Prediction.ipynb
```

Run the notebook cells sequentially.

---

## Model Saving

The notebook saves:

* Trained models
* Preprocessing pipelines
* Encoders and transformers
* Serialized artifacts using Joblib/Pickle

Example:

```python
joblib.dump(model, 'model.pkl')
```

---

## Inference

The notebook includes an inference section for predicting accident hotspots on new incoming data.

Typical inference workflow:

1. Load saved model
2. Load preprocessing artifacts
3. Transform new input data
4. Generate predictions
5. Visualize or export results

---

## Example Use Cases

* Smart city traffic monitoring
* Urban planning
* Road safety analysis
* Emergency response optimization
* Insurance risk assessment
* Accident prevention systems

---

## Future Improvements

Potential enhancements:

* Real-time accident prediction
* Deep learning approaches
* Live traffic integration
* Weather API integration
* GPS and IoT sensor data support
* Deployment as a web application
* Cloud deployment pipeline

---


## License

This project is intended for educational and research purposes.

You may modify and use it according to your project requirements.
