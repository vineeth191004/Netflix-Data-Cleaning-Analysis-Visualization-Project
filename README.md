# 🎬 Netflix Data Cleaning, Analysis & Visualization

## 📘 Project Overview
This project explores and analyzes the **Netflix titles dataset**, containing detailed information about movies and TV shows available on the platform.  
The goal is to **clean**, **analyze**, and **visualize** the dataset to identify trends in content type, ratings, genres, countries, and other attributes.

---

## 🧠 Objectives
- Perform comprehensive **data cleaning** using Python (Pandas).
- Conduct **exploratory data analysis (EDA)** to extract meaningful insights.
- Visualize patterns in Netflix content such as type, ratings, and release year.
- Prepare a cleaned dataset for future **machine learning or Tableau dashboards**.

---

## 🧰 Tools & Technologies
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, WordCloud  
- **IDE / Environment:** Visual Studio code

---

## 📊 Dataset Description
The dataset contains records of movies and TV shows from Netflix, with each row representing a unique title.

| Column | Description |
|--------|--------------|
| `show_id` | Unique ID for each title |
| `type` | Movie or TV Show |
| `title` | Title name |
| `director` | Name of the director |
| `country` | Country of origin |
| `date_added` | Date when the title was added to Netflix |
| `release_year` | Year of original release |
| `rating` | Audience rating (e.g., TV-MA, PG-13) |
| `duration` | Duration (minutes or number of seasons) |
| `listed_in` | Genres or categories |

---

## 🧹 Data Cleaning Process
1. **Loaded** the dataset using Pandas.  
2. **Normalized column names** to lowercase and snake_case format.  
3. **Handled missing values**:
   - Filled missing `director` and `country` with `"Unknown"`.
   - Converted placeholders like `"N/A"`, `"Not Given"` → `NaN`.
   - Dropped duplicate rows.
4. **Parsed key fields**:
   - Converted `date_added` → datetime.
   - Converted `release_year` → integer.
   - Extracted duration values (`duration_value`) and type (`duration_unit`).
5. **Split multiple genres** from `listed_in` into lists for flexible analysis.
6. Created new columns:
   - `num_genres`: Number of genres per title.
   - `duration_value` & `duration_unit`.

---

## 📊 Exploratory Data Analysis (EDA)
Key questions explored:
- How many **movies vs. TV shows** are on Netflix?
- Which **countries** produce the most content?
- What are the **most common ratings**?
- Which **genres** dominate the catalog?
- Who are the **top directors**?
- How has Netflix’s content **grown over time**?

---

## 📈 Visualizations
The following visualizations were created using Matplotlib and Seaborn:

- 📦 Count of Movies vs TV Shows  
- 🎯 Distribution of Ratings  
- 🌎 Top 15 Countries by Number of Titles  
- 📆 Titles Added per Year  
- 🎭 Top Genres by Frequency  
- 🎬 Top Directors  
- ☁️ WordCloud of Movie Titles  
- 📈 Monthly Trends of Movies and TV Shows  

---

## 💡 Key Insights
- **Movies dominate** Netflix’s catalog compared to TV Shows.  
- The **United States** leads in content production, followed by the **United Kingdom** and **India**.  
- **TV-MA** and **TV-14** are the most common ratings, suggesting mature content is popular.  
- **Dramas, Comedies, and Documentaries** are among the most frequent genres.  
- There’s a clear **growth trend** in titles added between 2018–2021.  
- The **average movie duration** is around 90–100 minutes.  

---

## 📁 Output Files
- `netflix_titles_cleaned.csv` → Cleaned dataset ready for Tableau or ML.  
- `netflix_summary.csv` → Summary of key statistics.  
- `Netflix_Data_Analysis.ipynb` → Jupyter Notebook with full code.  

