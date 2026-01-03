
# IBM Data Science Professional Capstone Project

## SpaceX Falcon 9 Landing Success Prediction

This project applies the complete data science workflow to predict SpaceX Falcon 9 first-stage landing outcomes. By analyzing historical launch data, the goal is to identify key factors influencing landing success and build a predictive model that determines whether a rocket will land successfully.

**Business Context:** SpaceX has disrupted the space industry by reusing first-stage boosters, reducing launch costs from ~$165M to $62M per mission. Accurately predicting landing success is crucial for cost estimation and mission planning.

![SpaceX Landing](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0701EN-SkillsNetwork/lab_v2/images/landing_1.gif)

---

## Key Results

- **Best Model Performance:** Logistic Regression \ SVM achieved **83.3% accuracy**
- **Temporal Trend:** Success rates improved from <40% (2013) to >80% (2020)
- **Launch Site Analysis:** KSC LC-39A showed highest success rate (76.9%)
- **Orbit Performance:** ES-L1, GEO, HEO, and SSO orbits demonstrated superior success rates
- **Payload Insights:** Lighter payloads (<5,500 kg) correlated with higher success probability

---

## Technical Implementation

### 1. Data Collection & Preparation
- **API Integration:** Queried SpaceX REST API for launch data (booster versions, payloads, outcomes)
- **Web Scraping:** Extracted complementary data from Wikipedia using BeautifulSoup
- **Data Cleaning:** Handled missing values, standardized formats, created feature variables

**Technologies:** Python, Requests, BeautifulSoup, Pandas

### 2. Exploratory Data Analysis
- **SQL Analysis:** Complex queries to identify patterns in launch sites, payload distributions, and temporal trends
- **Statistical Visualization:** Correlation analysis between payload mass, orbit type, and success rates
- **Geospatial Analysis:** Interactive Folium maps analyzing launch site proximity to infrastructure and equator

**Technologies:** SQLite, Matplotlib, Seaborn, Folium

### 3. Machine Learning Pipeline

**Methodology:**
- Feature standardization using StandardScaler
- Train-test split (80/20)
- GridSearchCV for hyperparameter optimization
- Confusion matrix evaluation
  
**mplemented and compared four classification algorithms:**
- **Logistic Regression          (best performer: 83.33%)**
- **Support Vector Machine (SVM) (best performer: 83.33%)**
- Decision Tree 
- K-Nearest Neighbors (KNN)

**Technologies:** Scikit-learn, NumPy
---
## Project Structure

| Notebook | Description |
|----------|-------------|
| `1_1_data-collection-api.ipynb` | SpaceX API data retrieval and JSON processing |
| `1_2_webscraping.ipynb` | Wikipedia data extraction via BeautifulSoup |
| `2_1_eda-sql.ipynb` | SQL-based exploratory analysis |
| `2_2_eda-visualization.ipynb` | Statistical visualizations and trend analysis |
| `3_1_launch-site-location.ipynb` | Interactive geospatial mapping with Folium |
| `4_1_machine-learning-prediction.ipynb` | Classification model development and evaluation |

---

## Skills Demonstrated

**Data Engineering:** API integration, web scraping, SQL queries, data cleaning  
**Analysis:** Exploratory data analysis, statistical inference, geospatial analysis  
**Machine Learning:** Classification algorithms, model evaluation, hyperparameter tuning  
**Visualization:** Matplotlib, Seaborn, Folium interactive maps  
**Tools:** Python, Jupyter, Pandas, NumPy, Scikit-learn

---

## Certification
## Code Files and Prasentation by Stefan Civelek
| IBM Data Science Professional | Applied Data Science Capstone |
|:---:|:---:|
| <!-- Bild 1 --> <a href="https://www.credly.com/badges/a561fe39-3415-433d-b9d2-0656b43e205c"><img src="https://images.credly.com/size/680x680/images/42ce4209-8839-431a-9046-f2ce2e72e04b/Coursera_20Data_20Science_20Professional_20Certificate.png" width="150"></a> | <!-- Bild 2 --> <a href="https://www.credly.com/badges/ffbf1bee-12a5-4363-bc53-7c70ec061ab7"><img src="https://images.credly.com/size/680x680/images/169512d3-cef6-43e3-bec8-e6af2723a076/image.png" width="150"></a> |

**Author:** Stefan Civelek  
**Repository:** [github.com/StefanC05/IBM_DataScience_Capstone](https://github.com/StefanC05/IBM_DataScience_Capstone)
