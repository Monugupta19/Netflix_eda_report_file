# Netflix Exploratory Data Analysis (EDA) Report 📊🎬

This project presents an **Exploratory Data Analysis (EDA)** of Netflix content data to understand trends in movies and TV shows, including genre patterns, release timeline growth, ratings distribution, and global content spread.

The analysis includes **data cleaning, preprocessing, visualization**, and **insight generation** using Python libraries.

---

## 📌 Project Objective

The goal of this Netflix EDA project is to:
- Explore Netflix’s content dataset structure
- Handle missing values and duplicates
- Analyze content attributes such as:
  - type (Movie/TV Show)
  - ratings
  - duration
  - genres
  - release year trends
  - content addition trends (month/year)
  - geographic distribution (country)
- Provide actionable insights and recommendations based on patterns in the data

---

## 🧾 Dataset Overview

- **Total Records:** 8,807  
- **Total Columns:** 12  
- **Data Types:**  
  - 11 Categorical columns  
  - 1 Numerical column  

---

## 🧩 Column Description

Key columns in the dataset:

| Column Name     | Description |
|----------------|-------------|
| show_id        | Unique ID for each title |
| type           | Movie / TV Show |
| title          | Name of the show/movie |
| director       | Director name(s) |
| cast           | Actor/actress names |
| country        | Production country |
| date_added     | Date Netflix added the title |
| release_year   | Original release year |
| rating         | Maturity rating (TV-MA, PG, etc.) |
| duration       | Movie minutes / TV seasons |
| listed_in      | Genres/categories |
| description    | Short summary of content |

---

## 🧹 Data Cleaning & Preprocessing

### ✅ Missing Values Check
Missing values were mostly found in:
- **director:** 2634
- **cast:** 825
- **country:** 831  
Minor missing values in:
- date_added
- rating
- duration

### ✅ Handling Missing Values
- Filled missing values in **director, cast, country, duration** with `"Unknown"`
- Dropped missing values from **rating** and **duration**
- Removed duplicates (if any)
- Renamed `listed_in` to `genres`
- Extracted and converted:
  - `year_added`
  - `month_added`

---

## 📈 Exploratory Data Analysis & Visualizations

This project includes multiple visualizations such as:

### 1️⃣ Genre Distribution (Top Genres)
**Key Insight:**
- Netflix is dominated by:
  - Dramas
  - Comedies
  - Documentaries  
These genres appear most frequently.

---

### 2️⃣ Content Release Trend by Year
**Key Insight:**
- Titles increase sharply after 2000
- Peak content between **2017–2020**
- Drop after 2020 likely due to **COVID-19 production delays**

---

### 3️⃣ Country-wise Content Distribution
**Key Insight:**
Top producing countries:
- United States
- India
- United Kingdom
- Japan  
Netflix shows strong focus on **North America + Asia**, with global expansion.

---

### 4️⃣ Monthly Content Addition Trend
**Key Insight:**
- Most content added in:
  - **July (highest)**
  - December & April  
- January shows the lowest additions.

---

### 5️⃣ Rating Distribution
**Key Insight:**
- **TV-MA** is the most common rating
- Netflix has strong focus on **adult and young-adult audience**
- Less focus on children content (TV-Y, G are fewer)

---

### 6️⃣ Movie Duration Trend
**Key Insight:**
- Most movies are between **80–120 minutes**
- High concentration around **90 minutes**
- Very long movies (150+ mins) are rare
- Netflix appears to prefer **short, easy-to-consume content**

---

### 7️⃣ TV Show Season Count
**Key Insight:**
- Most TV shows have only **1 season**
- Multi-season shows (5+ seasons) are rare  
Netflix focuses heavily on **limited series & short-format shows**

---

### 8️⃣ Genre Trends Over Time
**Key Insight Highlights:**
- Genre diversity increases significantly after 2015
- Rapid rise in international content after 2018
- Documentary releases steadily increase
- Drama remains dominant
- Crime genre popularity grows strongly after 2016
- Big spike in 2020 due to increased streaming usage during the pandemic

---

## 📌 Conclusion (Key Findings)

- Netflix content is mostly modern (median release year ~2017)
- Movies dominate slightly more than TV shows
- User preferences are concentrated around few genres (Drama, Comedy, Action, Documentary)
- Netflix has heavily expanded globally, especially in international content
- Strong maturity rating trend (TV-MA & TV-14 increasing)

---

## ✅ Recommendations

- **Focus on high-performing genres** (Drama, Comedy, Action, Documentaries)
- Improve personalization:
  - Recommend niche genres to relevant audiences
- Increase variety within popular genres:
  - (e.g., Drama-Romance, Action-Thriller)

---

## 🛠 Tools & Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Plotly
- Google Colab

---

## 📄 Report File

The full EDA report is available in the repository:

📌 `Netflix_eda_report.pdf`

---

## 👤 Author

**Monu Gupta**  
📧 monugupta8758@gmail.com  

---

⭐ If you found this project useful, don’t forget to give it a **star**!
