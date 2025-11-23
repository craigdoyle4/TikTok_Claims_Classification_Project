# 📊 TikTok Claim Classification Project  
**Data Analytics • Statistical Testing • Regression Modelling • Machine Learning**

🔗 **Presentation Link:**  
https://www.canva.com/design/DAG1rb0DMKk/21FpYJwvgMigI2pn2RGS5Q/edit?utm_content=DAG1rb0DMKk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

---

## 📁 Project Overview
This project investigates how TikTok videos differ in engagement and characteristics depending on whether they contain *claims* or *opinions*.  
Using a dataset of **19,000+ TikTok videos**, I applied data cleaning, exploratory analysis, hypothesis testing, regression modelling, and advanced machine learning to understand and classify content patterns.

The project follows the structured progression of the IBM Data Analyst curriculum:

- **Course 2:** Data cleaning & preparation  
- **Course 3:** Tableau exploratory dashboards  
- **Course 4:** Hypothesis testing  
- **Course 5:** Logistic regression modelling  
- **Course 6:** Machine learning classification (Random Forest & XGBoost)

---

## 📦 Dataset Description
Each TikTok entry includes:

- `claim_status` (claim or opinion)  
- `verified_status` (verified or not verified)  
- `author_ban_status`  
- `video_duration_sec`  
- `video_transcription_text`  
- Engagement metrics:  
  - `video_view_count`  
  - `video_like_count`  
  - `video_share_count`  
  - `video_download_count`  
  - `video_comment_count`

Total rows: **19,382**

---

## 🧹 1. Data Cleaning & Preparation
Performed using Python (Pandas & NumPy):

- Removed missing values and duplicates  
- Inspected and cleaned all feature types  
- Encoded categorical variables  
- Engineered new numerical/text indicators  
- Applied train–test split for modelling  

---

## 📊 2. Exploratory Data Analysis (EDA)
Tableau was used to explore:

- Views, likes, shares, comments  
- Claim vs. opinion content  
- Author ban status  
- Distribution of engagement metrics  
- Boxplots & scatterplots for engagement patterns  

**Key Insights:**

- Opinion videos came *only* from active users  
- Claim videos received **significantly more views & likes**  
- Engagement distributions were **heavily right-skewed**  
- Shorter videos tended to receive higher engagement  

---

## 🧪 3. Hypothesis Testing
A two-sample **t-test** was used to compare the mean view counts of verified vs. not verified videos.

- **Null hypothesis (H₀):** No difference in engagement  
- **Result:** *p < 0.05*  
- **Conclusion:** Verified/claim content receives significantly higher engagement

This validated the insights found in the EDA.

---

## 📈 4. Logistic Regression Modelling (Course 5)
Built a logistic regression model to classify videos as verified or not verified based on engagement and content features.

### Steps:
- One-hot encoding for categorical variables  
- Standardisation of predictors  
- Model training & evaluation via:  
  - Confusion matrix  
  - Classification report  
  - Coefficient interpretation  

### Accuracy:
**~65%**

### Insights from coefficients:
- **Longer durations** → increased chance of verification  
- **More shares** → strong positive influence  
- **High comment/download counts** → negative effect  
- Engagement metrics were highly correlated predictors  

---

## 🤖 5. Machine Learning Models (Course 6)

### 🔹 Random Forest Classifier
- **Cross-validated accuracy:** **99.95%**  
- **Validation accuracy:** **100%**  
- Best performing model in the project  

### 🔹 XGBoost Classifier
- **Cross-validated accuracy:** **98.98%**  
- **Validation accuracy:** **~99%**

These models significantly outperformed logistic regression and captured complex, non-linear relationships in the data.

---

## 🧠 Key Findings
- Claim videos consistently outperform opinions in engagement metrics  
- Statistical testing confirmed significant differences in mean engagement  
- Logistic regression provided interpretability but limited accuracy  
- Tree-based models (RF, XGBoost) achieved near-perfect classification  
- Adding text-based features improved model depth  
- TikTok engagement patterns can be reliably modelled with ML  

---

## 🛠️ Technologies Used
- **Python:** pandas, numpy, seaborn, matplotlib  
- **Machine Learning:** scikit-learn, xgboost  
- **Feature Engineering:** CountVectorizer  
- **Visualisation:** Tableau  
- **Statistics:** SciPy  



