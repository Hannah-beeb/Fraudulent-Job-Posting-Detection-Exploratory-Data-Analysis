# Fraudulent-Job-Posting-Detection-Exploratory-Data-Analysis

This project explores the Fraudulent Job Posting Detection dataset using detailed Exploratory Data Analysis (EDA) techniques to understand patterns that differentiate real vs. fake job postings.
The focus is on data cleaning, feature engineering, and insights from visualizations.


.

📊 Dataset Description

The dataset used in this project is a real-world collection of online job postings gathered from various employment platforms. It contains both legitimate and fraudulent job advertisements, making it suitable for analyzing patterns associated with job posting fraud.

Each record in the dataset represents a single job posting and includes detailed information related to the job role, company, location, and required qualifications. The dataset is highly heterogeneous, consisting of categorical, textual, and binary features, which makes it ideal for Exploratory Data Analysis.

🔹 Key Characteristics of the Dataset
Nature of Data: Real-world, noisy, and unbalanced
Total Records: Several thousand job postings
Data Types: Categorical (employment type, industry, job function)
Binary (telecommuting, fraudulent)
Text-based (job title, location)
Target Variable: fraudulent
0 → Real job posting
1 → Fraudulent job posting

🧹 Data Cleaning Performed

✔ Handling Missing Data
Columns with >60% missing values were dropped.
Remaining missing values were filled using:
"Unknown" → text fields
"Not Specified" → categorical fields

✔ Encoding
Converted fraudulent → fraud_label (0 = Real, 1 = Fake)

✔ Other Cleaning
Removed duplicates

type

📈 Exploratory Data Analysis (EDA)

The EDA includes:

1️⃣ Univariate Analysis

Countplots for:
employment type
required experience
job function

2️⃣ Bivariate Analysis

Fraud rate vs:
telecommuting
job function
employment type
job industry

3️⃣ Multivariate Analysis

Correlation heatmap
Cluster heatmap
Grouped barplots

size

🔍 Key Insights From EDA

Fraud postings tend to have shorter job descriptions and minimal requirements.
Fake postings usually do not include company logos.
Fraud rate is higher in remote / telecommuting jobs.
Text-length features show clear separation between real and fake posts.
Many fraud indicators appear together → multivariate patterns are stron.



🧠 Recommendations for Job Portals

Flag postings missing:
Company logo
Company profile
Proper job description
Add stronger verification for remote jobs.
Encourage employers to fill complete information fields.

🛠 Tools & Libraries Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook

📄 Report

A complete PDF report of the analysis is included:
EDA Report.pdf


🚀 How to Run the Notebook
pip install -r requirements.txt
jupyter notebook

⭐ Support
If you find this helpful, consider starring ⭐ the repository!
