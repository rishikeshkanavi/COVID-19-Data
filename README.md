# COVID-19 Data Analysis Project

A comprehensive exploratory data analysis (EDA) project focused on
understanding global COVID-19 trends using Python and Pandas.

------------------------------------------------------------------------

## 📋 Table of Contents

-   Project Overview
-   Project Structure
-   Dataset
-   Data Cleaning & Preprocessing
-   Data Analysis
-   Key Insights
-   Getting Started
-   Prerequisites
-   Usage
-   Future Improvements

------------------------------------------------------------------------

## 🎯 Project Overview

This repository contains a COVID-19 data analysis notebook that
performs:

-   Data loading and preprocessing\
-   Cleaning and transformation\
-   Country-wise case aggregation\
-   Date-wise trend analysis\
-   Filtering high confirmed case records

The project demonstrates practical skills in data wrangling,
aggregation, and exploratory data analysis using Pandas.

------------------------------------------------------------------------

## 📁 Project Structure
```
COVID19-Data-Analysis/ 
├── data/ 
│   └── covid_19_data.csv
├── notebook/ 
│   └── covid_analysis.ipynb
|   └── README.md
```


------------------------------------------------------------------------

## 📊 Dataset

### COVID-19 Dataset (covid_19_data.csv)

Format: CSV\
Description: Global COVID-19 case data

Key Fields: - SNo - ObservationDate - Province/State - Country/Region -
Confirmed - Deaths - Recovered - Last Update

------------------------------------------------------------------------

## 🧹 Data Cleaning & Preprocessing

The following steps were performed:

-   Dropped unnecessary columns: SNo, Last Update\
-   Renamed columns for clarity\
-   Converted Date column to datetime format\
-   Filled missing values

------------------------------------------------------------------------

## 📈 Data Analysis

### Country-wise Aggregation

df.groupby('Country')\[\['Confirmed','Deaths','Recovered'\]\].sum()

### Country + Date-wise Aggregation

df.groupby(\['Country','Date'\])\[\['Confirmed','Deaths','Recovered'\]\].sum()

### Filtering High Case Records

df3 = df2\[df2\['Confirmed'\] \> 100\]

------------------------------------------------------------------------

## 🔍 Key Insights

-   Significant variation in case numbers across countries\
-   Progressive increase in confirmed cases over time\
-   Aggregation helps identify high-impact regions

------------------------------------------------------------------------

## 🚀 Getting Started

Clone the repository:

git clone `<repository-url>`{=html} cd COVID19-Data-Analysis

Install dependencies:

pip install pandas numpy jupyter

Run Jupyter Notebook:

jupyter notebook

------------------------------------------------------------------------

## 🚀 Future Improvements

-   Add data visualizations\
-   Perform time-series forecasting\
-   Create interactive dashboards\
-   Deploy as web dashboard

------------------------------------------------------------------------

Version: 1.0.0\
Status: Completed (Basic EDA Phase)
