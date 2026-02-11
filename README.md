**🦠 COVID-19 Data Analysis using Python
**
A beginner-friendly data analysis project that explores COVID-19 dataset trends using Pandas and NumPy.
This notebook focuses on data cleaning, preprocessing, aggregation, and filtering to understand country-wise and date-wise COVID-19 statistics.

**📌 Project Overview
**
This project performs:

📥 Data loading from CSV

🧹 Data cleaning and preprocessing

📊 Exploratory Data Analysis (EDA)

🌍 Country-wise case aggregation

📅 Date-wise trend analysis

🔎 Filtering high confirmed case records

The goal is to understand how COVID-19 cases are distributed across countries and over time.

**📂 Dataset Used
**
File: covid_19_data.csv

The dataset contains:

Observation Date

Province/State

Country/Region

Confirmed Cases

Deaths

Recovered Cases

Last Update

⚙️ Technologies Used

🐍 Python

📊 Pandas

🔢 NumPy

📒 Jupyter Notebook

🧹 Data Preprocessing Steps

The following cleaning steps were performed:

Dropped unnecessary columns:

SNo

Last Update

Renamed columns:

ObservationDate → Date

Province/State → Province

Country/Region → Country

Converted Date column to datetime format

Filled missing values with "NA"

📊 Data Analysis Performed
1️⃣ Dataset Overview

.head()

.describe()

.info()

2️⃣ Country-wise Aggregation
df.groupby('Country')[['Confirmed','Deaths','Recovered']].sum()

✔ Calculates total confirmed, deaths, and recovered cases per country.

3️⃣ Country + Date-wise Aggregation
df.groupby(['Country','Date'])[['Confirmed','Deaths','Recovered']].sum()

✔ Helps analyze trends over time for each country.

4️⃣ Filtering High Case Records
df3 = df2[df2['Confirmed'] > 100]

✔ Filters records where confirmed cases exceed 100.

📈 Key Insights

Countries show significant variation in total confirmed cases.

Case counts increase progressively over time.

Filtering allows identification of high-risk periods or countries.

🚀 How to Run This Project

Clone the repository:

git clone https://github.com/your-username/your-repo-name.git

Navigate to the project folder:

cd your-repo-name

Install required libraries:

pip install pandas numpy

Open the Jupyter Notebook:

jupyter notebook

Run all cells.

📌 Future Improvements

📈 Add data visualizations (Matplotlib / Seaborn)

🌎 Create interactive dashboards

🤖 Add predictive modeling

📊 Perform trend forecasting

🎯 Learning Outcome

Through this project, I learned:

Data cleaning techniques

Pandas groupby operations

Aggregation & filtering

Basic exploratory data analysis

📄 License

This project is for educational purposes.
