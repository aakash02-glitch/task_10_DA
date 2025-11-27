# Naukri Data Analyst Jobs – Scraping Logic, Cleaning & Analysis

## 📌 Overview

This project uses a Kaggle dataset containing Naukri Data Analyst job listings. It demonstrates the full workflow of simulated scraping logic, data cleaning, skill extraction, and exploratory job market analysis.

## 📂 Dataset Columns

* Job Role
* Company
* Job Type
* Location
* Experience
* Salary per annual
* Description
* Key Skills
* Posted on
* Apply link

## 🕸️ Scraping Logic (Used to Create the Dataset)

The original dataset was created using:

* `find_all()` / `select()` for extracting repeated job cards
* `.text.strip()` for cleaning text fields
* Extraction of Job Role, Company, Job Type, Location, Experience, Salary, Description, Key Skills, Posted Date, and Apply Link

This resulted in a structured dataset suitable for data analysis.

## 🧹 Data Cleaning Performed

* Trimmed text using `.str.strip()`
* Standardized text to lowercase
* Cleaned salary values using regex → `Cleaned_Salary`
* Extracted experience years using regex → `Experience_Years`
* Split and normalized skills using regex (`[,/|•]`)
* Created skill lists and frequency counts using `Counter`

## 📊 Analysis Performed

* Total jobs scraped
* Top hiring locations
* Most in-demand skills
* Distribution of job types
* Bar chart visualization of top 5 locations

## 🧠 Key Insights

* Major hiring hubs identified
* SQL, Python, Excel, Power BI, Tableau emerged as top skills
* Experience requirements vary widely across companies

## ⚠️ Challenges Faced

* Dynamic content loading
* Inconsistent salary and experience formats
* Mixed skill separators (comma, slash, bullets)
* Missing fields in some listings

## ▶️ How to Run

1. Clone the repository
2. Place the dataset file: `Naukri_Data_Analyst_Jobs.csv`
3. Run the Jupyter Notebook
4. Install dependencies:

```
pip install pandas matplotlib
```

## 📁 Files Included

* Jupyter Notebook
* Cleaned dataset
* Visualizations
* Report summary

## 📜 License

This project is for educational and analytical purposes.

---

Feel free to ask if you want a **PDF**, **PowerPoint**, or a **LinkedIn post** too!
