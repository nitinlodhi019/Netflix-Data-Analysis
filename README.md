# Netflix Content Strategy Analysis

This repository contains a comprehensive analysis of the Netflix dataset, performed within a Python Jupyter Notebook. The goal of this project is to explore the Netflix content library and provide data-driven recommendations to inform content acquisition, production, and marketing strategies.

## Project Goal

To analyze the Netflix dataset to answer key business questions related to content strategy, user demographics, and market growth. The final output is a set of actionable, data-backed recommendations for executive-level stakeholders.

**Tools Used**

* Python 3

* Pandas: For data loading, cleaning, and manipulation.

* Matplotlib & Seaborn: For data visualization and generating plots.

* WordCloud: For visualizing text data from movie/show titles.

* Jupyter Notebook: As the primary development environment.

## Dataset

This project uses a public dataset of Netflix titles (as of 2021), available from sources like Kaggle. The dataset includes information such as:

* show_id, type (Movie/TV Show)

* title, director, cast

* country, date_added, release_year

* rating, duration, listed_in (genres)

## description

**Project Workflow**

1. Data Loading: Imported the netflix.csv file into a Pandas DataFrame.

2. Data Cleaning & Preprocessing:

  * Handled missing values by filling director, cast, and country with "Unknown" to preserve data.
  
  * Dropped a small number of rows with critical missing data (date_added, rating).
  
  * Removed duplicate entries.
  
  * Corrected data types, including converting date_added to datetime (and stripping hidden whitespace that caused errors).
  
  * Feature Engineering: Parsed the duration column into two new numerical columns: duration_min for movies and duration_seasons for TV shows.

3. Exploratory Data Analysis (EDA): Answered 20 key business questions through extensive data visualization.

4. Insights & Recommendations: Summarized the findings into a strategic report.

## Key Questions & Analysis

This analysis was structured to answer 20 specific questions across five key business areas.

1. Content Strategy
   
  * What is the ratio of Movies vs. TV Shows on Netflix?
  
  * Which genres are most popular globally?
  
  * Which years saw the highest release of content?
  
  * Which countries produce the most content?
  
  * How has the trend of adding new content evolved?

2. User Demographics & Targeting
   
  * Which ratings (e.g., TV-MA, PG) are most frequent?
  
  * Do some countries produce more mature (TV-MA) content?
  
  * Which genres are more associated with TV Shows vs. Movies?
  
  * Which genres dominate the U.S. vs. other countries?
  
  * What genres are most popular in the last 3 years?

3. Talent Acquisition & Partnerships
   
  * Who are the top 10 directors with the most content?
  
  * Which actors appear most frequently?
  
  * Which director-genre pairs are most frequent?
  
  * How many titles have unknown directors or cast?

4. Duration & Engagement
   
  * What is the average duration of Movies?
  
  * What’s the most common number of seasons for TV shows?
  
  * Is there a trend in movie durations over the years?

5. Content Launch Strategy
   
  * In which months does Netflix add the most content?
  
  * How does the genre distribution vary across different years?
  
  * Which countries produce the most content in each genre?

## Key Insights & Recommendations

The analysis revealed a clear, decisive shift in content strategy and identified several key opportunities.

1. The Strategic Pivot: "TV Show-First"

**Insight:** While the total library is ~70% movies, this is historical. Since 2018, the number of new TV shows added has grown rapidly, while new movies added has declined. Netflix is now a TV Show-first platform.

**Recommendation:** Prioritize budget and production resources for original TV shows, as this is the clear strategic growth driver.

2. The 1-Season Reality: "The Limited Series Model"
   
**Insight:** The vast majority of TV shows on the platform have only one season. This suggests a high churn rate or a deliberate strategy of producing single-season arcs.

**Recommendation:** Formalize this by embracing a "Limited Series" strategy. This lowers financial risk, attracts top-tier talent for short-term commitments, and keeps the content pipeline feeling fresh.

3. The Growth Engine: "Global & Local"
   
**Insight:** The US market is mature. The largest growth opportunity is international, with "International Movies" being a top genre and countries like India, South Korea, and Japan being key producers.

**Recommendation:** Shift from acquiring generic "international" content to producing "local-first" content for high-growth markets, using local directors and actors to ensure authenticity.

4. The "Primetime" Launch Window
   
**Insight:** There is a massive, consistent spike in new content added every year between October and January.

**Recommendation:** Align major TV show launches with this existing "primetime" window to capitalize on user behavior and existing marketing momentum.

## How to Run This Project

* **Clone the repository:**
```
git clone  
```

**Install the required libraries:**
```
pip install pandas matplotlib seaborn wordcloud jupyter
```

* Launch Jupyter Notebook:

* jupyter notebook

* Open the Netflix_analysis.ipynb file and run the cells.
