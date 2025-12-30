# IBM Data Science Professional Certificate - Capstone Project

## About the Course

The IBM Data Science Professional Certificate is a comprehensive program offered through Coursera that covers the foundational skills required for a career in data science. The course includes hands-on training in Python, SQL, data visualization, statistical analysis, and machine learning. Participants work with real-world datasets and tools like Jupyter Notebooks, pandas, NumPy, scikit-learn, and various visualization libraries to develop practical data science skills.

## Capstone Project: SpaceX Falcon 9 Launch Success Prediction
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0701EN-SkillsNetwork/lab_v2/images/landing_1.gif)

This capstone project analyzes SpaceX Falcon 9 rocket launches to predict landing success rates. SpaceX has revolutionized space travel by making rocket launches significantly more cost-effective - a Falcon 9 launch costs approximately $62 million compared to competitors. The key to this cost reduction is the reusability of the first stage booster.

The project employs the complete data science workflow: data collection, wrangling, exploratory data analysis (EDA), interactive visualizations, and predictive modeling using classification algorithms. The goal is to determine the factors that influence successful rocket landings and build a model that can predict landing outcomes.

**Key findings:**
- Launch success rates improved significantly over time, reaching over 80% by 2020
- KSC LC-39A was the most successful launch site with a 76.9% success rate
- Orbits ES-L1, GEO, HEO, and SSO showed the highest success rates
- Lighter payloads generally performed better than heavier ones
- The Decision Tree classifier achieved the best prediction accuracy at 94.44%

---

## Project Files

### [1.1 Data Collection - SpaceX API](./1_1_jupyter-labs-spacex-data-collection-api.ipynb)

This notebook demonstrates data collection from the SpaceX REST API. The process involves requesting launch data in JSON format, extracting relevant information about rocket types, payloads, launch details, and landing outcomes, then converting this data into a structured pandas DataFrame for further analysis.

### [1.2 Data Collection - Web Scraping](./1_2_jupyter-labs-webscraping.ipynb)

This notebook uses BeautifulSoup to scrape Falcon 9 launch data from Wikipedia. The HTML response is parsed to extract tabular data about historical launches, which is then normalized and stored in CSV format to complement the API-collected data.

### [2.1 Exploratory Data Analysis - SQL](./2_1_jupyter-labs-eda-sql-coursera_sqllite.ipynb)

SQL queries are used to explore the dataset and answer specific questions about launch patterns. Analysis includes identifying unique launch sites, filtering launches by location prefix, calculating payload statistics for different booster versions, determining first successful landing dates, and ranking landing outcomes by time period.

### [2.2 Exploratory Data Analysis - Visualization](./2_2_jupyter-labs-eda-visualization.ipynb)

This notebook creates visual representations of the data using matplotlib and seaborn. Scatter plots examine relationships between variables, bar charts compare categorical data, and line charts reveal trends over time. Key insights include the correlation between payload mass and success rate, launch site performance, and temporal success patterns.

### [3 Interactive Map Analysis - Folium](./3_1_lab_jupyter_launch_site_location.ipynb)

Folium is used to create interactive maps showing launch site locations and their proximity to important geographical features. The maps display markers for each launch site with success/failure indicators, circles showing proximity zones, and lines measuring distances to coastlines, railways, and other infrastructure. This analysis reveals that sites closer to the equator offer fuel-saving advantages.

### [4 Machine Learning Prediction](./4_1_SpaceX_Machine_Learning_Prediction.ipynb)

The final notebook implements classification models to predict landing success. After data preprocessing including feature standardization and train-test splitting, four algorithms are trained and evaluated: Logistic Regression, Support Vector Machine (SVM), Decision Tree, and K-Nearest Neighbors (KNN). Model performance is compared using accuracy metrics and confusion matrices. The Decision Tree classifier achieved the highest accuracy at 94.44%, correctly predicting 12 successful landings and 5 failures in the test set.

---

## Code Files and Prasentation by Stefan Civelek
| IBM Data Science Professional | Applied Data Science Capstone |
|:---:|:---:|
| <!-- Bild 1 --> <a href="https://www.credly.com/badges/a561fe39-3415-433d-b9d2-0656b43e205c"><img src="https://images.credly.com/size/680x680/images/42ce4209-8839-431a-9046-f2ce2e72e04b/Coursera_20Data_20Science_20Professional_20Certificate.png" width="150"></a> | <!-- Bild 2 --> <a href="https://www.credly.com/badges/ffbf1bee-12a5-4363-bc53-7c70ec061ab7"><img src="https://images.credly.com/size/680x680/images/169512d3-cef6-43e3-bec8-e6af2723a076/image.png" width="150"></a> |


## Repository
Full project code and documentation: [https://github.com/StefanC05/DataScience_Capstone/tree/main](https://github.com/StefanC05/DataScience_Capstone/tree/main)
