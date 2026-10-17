# EDA-on-Amazon-Prime-Video
This EDA project analyzes the Amazon Prime Video TV Shows and Movies dataset to uncover trends in content type, genres, ratings, release years, and production countries. The goal is to generate insights into audience preferences, content distribution, and business opportunities through data visualization and analysis.

# 🎬 Amazon Prime Video Data Analysis & Insights
An end-to-end exploratory data analysis (EDA) and data processing project exploring Amazon Prime Video's content catalog. This project analyzes content trends, genre distributions, release patterns, ratings, and runtime statistics to understand streaming dynamics and catalog curation strategies.

## 📖 Overview
Amazon Prime Video hosts an extensive catalog of movies and television shows across diverse regions and genres. The goal of this project is to clean, transform, and analyze the catalog data to identify:
- Catalog composition (Movies vs. TV Shows ratio).
- Top-producing countries and localized content trends.
- Content rating segmentation and target audience demographics.
- Evolution of release patterns across decades.
- Common genres, key directors, and cast distribution.

## 📊 Dataset Summary
- **Source:** Amazon Prime Video Catalog Dataset
- **Features Analyzed:**
  - `show_id`: Unique identifier for each title
  - `type`: Category (`Movie` or `TV Show`)
  - `title`: Name of the movie/show
  - `director`: Primary director(s)
  - `cast`: Main cast members
  - `country`: Country of production
  - `date_added`: Date the title was added to Prime Video
  - `release_year`: Original release year of the content
  - `rating`: Target maturity rating (e.g., `TV-MA`, `PG-13`, `TV-14`, `R`, `All`)
  - `duration`: Runtime (in minutes for movies, seasons for TV shows)
  - `listed_in`: Associated genres/categories
  - `description`: Plot synopsis
    
## 🎯 Key Objectives & Questions Explored
1. **Content Mix:** What proportion of the catalog consists of Movies vs. TV Shows?
2. **Growth Trends:** In which years did the volume of released content peak?
3. **Regional Focus:** Which countries contribute the highest volume of titles to the platform?
4. **Maturity & Audience:** What are the most common content ratings, and what demographic is primary?
5. **Genre Landscape:** What genres dominate the library (e.g., Drama, Comedy, Documentaries, Action)?
6. **Runtime Analysis:** What is the average duration of movies compared to seasons per TV series?

## 🛠 Tech Stack & Libraries
- **Language:** Python
- **Environment:** Google Colab / Jupyter Notebook
- **Core Libraries:**
  - `pandas` – Data manipulation, imputation, and structural inspection
  - `numpy` – Numerical transformations and array handling
  - `matplotlib` & `seaborn` – Statistical visualizations, histograms, and heatmaps
  - `re` / Text Handling – Parsing multi-value strings (`listed_in`, `cast`, `director`)

  ## 🔄 Project Workflow
  1. **Data Cleaning & Handling Missing Values:**
   - Handled missing values in `director`, `cast`, and `country` (imputed with `'Unknown'` or analyzed conditionally).
   - Standardized date formats for temporal extraction (`month_added`, `year_added`).
2. **Feature Engineering:**
   - Split and unnested comma-separated columns (`listed_in` genres, `country`, `cast`).
   - Parsed `duration` into numerical units: `movie_duration_min` and `tv_seasons_count`.
3. **Exploratory Data Analysis (EDA):**
   - Univariate and bivariate analysis on categorical and numerical variables.
   - Temporal trend tracking using grouped aggregations.
     
## 💡 Key Insights & Findings
*(Update values based on your exact notebook figures)*
- **Catalog Breakdown:** Movies constitute the majority (~70-80%) of the catalog, while TV series represent the remainder.
- **Top Genres:** Drama, Comedy, and Action/Suspense lead total catalog volume.
- **Content Growth:** A noticeable acceleration in added titles occurred from 2015 onwards, mirroring the streaming industry's digital expansion.
- **Audience Rating:** Titles categorized for mature/young adult audiences (`TV-MA`, `16+`, `18+`) hold significant presence, alongside general family entertainment.
- **Runtime Distribution:** The median movie duration sits around 90–105 minutes, while the vast majority of TV shows run for 1 to 2 seasons.

## 📈 Visualizations
The notebook includes detailed visualizations covering:
- **Bar Plots & Donut Charts:** Distribution of Movies vs. TV Shows.
- **Line Charts:** Yearly trend of content releases and catalog additions.
- **Countplots:** Top 10 countries by content production.
- **Histograms & KDE:** Runtime distribution for feature films.
- **Correlation/Frequency Tables:** Co-occurrence of top genres.

---

## 🔄 Project Workflow
