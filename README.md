# ⚡ energy-consumption-mlp: London Electrical Consumption Predictor

A data science project designed to predict the daily total electrical consumption of customers in each London borough. 

Developed for a fictional London energy company, this project joins historical weather and energy datasets to deliver predictive business insights through deep learning models.

## 🚀 Key Features

* **Advanced Preprocessing:** Handles missing data, formats data types, and identifies outliers. 
* **Feature Engineering:** Applies one-hot encoding to categorical text, standardizes numerical data, and extracts new time-based features (week, day, and year) from date columns. Redundant variables are dropped to improve model speed and performance.
* **Deep Learning Dynamics:** 
    * **Regression Tasks:** Implements the 'gelu' activation function.
    * **Classification Tasks:** Implements the 'softmax' activation function.
* **Comprehensive EDA:** Utilizes heatmaps, scatter plots, and histograms to identify key trends and data patterns.
* **Project Management:** Follows the Waterfall methodology, using Microsoft Project and Gantt charts to allocate tasks across the Project Manager, Data Analyst, and Data Scientist roles.

## 🛠️ Tech Stack

* **Environment:** Google Colab (utilizing built-in version control)
* **Data Processing:** Pandas, Numpy
* **Visualization:** Matplotlib, Seaborn

## 🧠 Methodology & Insights

The project utilizes a structured 7-stage data science lifecycle:
1.  **Business Understanding:** Defining the core problem.
2.  **Data Collection:** Reading CSV datasets within Google Colab.
3.  **Data Cleaning:** Handling missing values and outliers.
4.  **Exploratory Data Analysis (EDA):** Uncovering statistical patterns. 
    *   *Insight:* Significant missing data exists in the `cloud_cover` and `snow_depth` columns.
    *   *Insight:* Strong positive correlation (0.85) between `global_radiation` and `sunshine`, and strong negative correlation (-0.74) between `cloud_cover` and `sunshine`.
    *   *Insight:* `global_radiation` is a significant driver for both maximum temperature (0.69) and mean temperature (0.64).
5.  **Feature Engineering:** Transforming and selecting the most impactful variables.
6.  **Modeling & Evaluation:** Training deep learning models.
7.  **Deployment & Communication:** Translating mathematical results into clear business recommendations.

## 📊 Performance

The models evaluate performance based on a 70:30 train/test data split.

* **Regression Metrics:** Mean Absolute Error (MAE) and Mean Absolute Percentage Error (MAPE).
* **Classification Metrics:** SparseCategoricalAccuracy.

## 📂 Datasets

* **London Weather Data:** Daily weather observations spanning from 1979 to 2021.
* **London Energy Data:** Hourly energy consumption dataset from 2011 to 2014.

## 💻 How to Run

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/winengewe/energy-consumption-mlp.git
    cd energy-consumption-mlp
    ```

2.  **Open the Environment:**
    Open `energy_consumption_mlp.ipynb` in Google Colab or your preferred Jupyter environment.

3.  **Mount Data & Install Dependencies:**
    Ensure Google Drive is mounted to securely read the necessary CSV datasets and that `pandas`, `numpy`, `matplotlib`, and `seaborn` are installed.

4.  **Execute the Pipeline:**
    Run the notebook cells sequentially to process the data, review visual insights, and evaluate the deep learning predictions.
```
