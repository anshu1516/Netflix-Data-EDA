# 🎬 Netflix Data — Exploratory Data Analysis (EDA) using Python

A comprehensive exploratory data analysis of Netflix's content library, answering 15 key business questions about content types, ratings, genres, countries, directors, actors, and growth trends.

---

## 📌 Project Overview

This project dives deep into the Netflix titles dataset to uncover patterns in content distribution, production trends, and viewer ratings. It covers everything from the most common genres and top-producing countries to the most frequent actors and year-wise content growth on the platform.

---

## 📂 Dataset

- **Source:** [Kaggle — Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- **File used:** `netflix_titles.csv`
- **Key columns:** `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description`

---

## 🧹 Data Cleaning

- Filled null values in `director`, `cast`, and `country` with meaningful placeholders
- Dropped rows with null values in `date_added`, `rating`, and `duration` (< 10% of data)
- Checked and confirmed no duplicate records
- Parsed `duration` column into numeric format for both movies (minutes) and TV shows (seasons)
- Converted `date_added` to datetime and extracted `year_added`

---

## 🔍 15 Business Questions Answered

| # | Question |
|---|---|
| 1 | How many records are in the dataset? |
| 2 | How many unique types (Movies / TV Shows) are present? |
| 3 | What is the distribution of content ratings (G, PG, TV-MA, etc.)? |
| 4 | What is the average duration of movies and TV shows? |
| 5 | Which director has the most content on Netflix? |
| 6 | Which country produces the most content on Netflix? |
| 7 | How has the number of content additions evolved over the years? |
| 8 | What are the top 5 countries with the highest number of rated content? |
| 9 | What are the most common genres listed in the dataset? |
| 10 | What are the oldest and newest releases on Netflix? |
| 11 | Who are the top 5 most frequent actors/actresses? |
| 12 | How many TV shows and movies were added to Netflix each year? |
| 13 | What is the distribution of release years for movies and TV shows? |
| 14 | What are the top 5 most common words in content descriptions? |
| 15 | Is there any correlation between release year and content rating? |

---

## 📊 Visualizations Included

- Count plot — Movies vs TV Shows
- Count plot — Rating distribution by content type
- Horizontal bar chart — Top 12 countries producing most content
- Line plot — Content additions per year
- Pie chart — Top 5 countries by rating count
- Pie chart — Top 10 most common genres
- Bar chart — Top 5 most frequent actors
- Grouped bar chart — Movies vs TV Shows added each year
- Side-by-side histograms — Release year distribution for Movies & TV Shows
- Bar chart — Top 5 most common words in descriptions

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| Pandas | Data loading, cleaning & manipulation |
| NumPy | Numerical operations |
| Matplotlib | Bar charts, pie charts & line plots |
| Seaborn | Count plots, histograms & bar plots |
| Collections (Counter) | Word & cast frequency counting |
| Google Colab | Development environment |

---

## 🚀 How to Run

### Option 1 — Open in Google Colab
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

*(Replace with your actual Colab notebook link)*

### Option 2 — Run Locally
```bash
git clone https://github.com/anshu1516/Netflix-Data-EDA.git
cd Netflix-Data-EDA

pip install pandas numpy matplotlib seaborn

jupyter notebook Case_study_Netflix_Data_EDA.ipynb
```

> **Note:** Download `netflix_titles.csv` from Kaggle and place it in the same directory before running.

---

## 💡 Key Insights

- **Movies** dominate Netflix's library compared to TV Shows
- The **United States** produces the most content on Netflix by a large margin
- **TV-MA** is the most common rating — Netflix leans towards mature content
- Content additions peaked around **2019-2020** before plateauing
- **International Movies** and **Dramas** are the most common genres
- There is **no significant correlation** between a title's release year and its rating

---

## 👤 Author

**Anshu** — [GitHub](https://github.com/anshu1516)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
