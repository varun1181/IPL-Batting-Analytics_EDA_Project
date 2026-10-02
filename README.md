# 🏏 IPL Batting Analytics (2008–2026)

An end-to-end data analytics project using Python to scrape, clean, explore, and visualize IPL batting statistics from ESPNcricinfo.

## 📌 Project Overview

This project analyzes IPL batting performance across seasons from 2008 to 2026. It uses web scraping to collect player statistics and exploratory data analysis (EDA) to identify trends in runs, batting average, strike rate, team contributions, and scoring milestones.

## 🎯 Objectives

- Collect season-wise IPL batting statistics using web scraping.
- Clean and structure raw HTML table data.
- Analyze player, team, and season performance.
- Explore relationships between runs and strike rate.
- Create visualizations and communicate data-driven insights.

## 🗂️ Dataset

- **Source:** ESPNcricinfo Statsguru
- **Coverage:** IPL seasons 2008–2026
- **Raw scraped rows:** 6,694
- **Player records after removing team-label rows:** 3,347
- **Unique players:** 805
- **Final columns:** 16

The dataset includes player, team, season, matches, innings, runs, highest score, batting average, balls faced, strike rate, centuries, fifties, ducks, fours, and sixes.

## 🛠️ Tools & Technologies

- Python
- Pandas and NumPy
- Requests and BeautifulSoup
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## ⚙️ Workflow

1. **Web Scraping:** Retrieved batting tables from ESPNcricinfo Statsguru, including paginated results across seasons.
2. **Data Understanding:** Inspected the dataset structure, data types, missing values, and duplicate records.
3. **Data Cleaning:** Removed team-label rows and an unwanted HTML artifact, renamed columns, converted data types, cleaned highest-score markers, and standardized team names.
4. **Missing Values:** Applied median imputation to missing numerical batting statistics.
5. **EDA:** Examined descriptive statistics, run distributions, player and team totals, season trends, strike rates, consistency, and outliers.
6. **Visualization:** Created charts using Matplotlib to communicate key patterns.
7. **Insights:** Summarized findings and recommendations based on the collected dataset.

## 📊 Key Findings

- **Highest cumulative runs by a player in the dataset:** V Kohli — 9,227.
- **Highest single-season run total in the dataset:** V Kohli — 973 runs in 2016.
- **Highest season total in the cleaned dataset:** 2026 — 27,425 runs.
- **Highest cumulative team runs in the cleaned dataset:** Mumbai Indians — 46,539.
- **Correlation between runs and strike rate:** approximately 0.416, indicating a moderate positive relationship.
- The run distribution is right-skewed, with a smaller number of records having high run totals.

> **Note:** These results are calculated from the cleaned dataset. Median imputation and the structure of player-season records can affect aggregate statistics, so the figures should not automatically be interpreted as official IPL totals.

## 📈 Visualizations

The project includes:

- Total IPL runs by season
- Top players by cumulative runs
- Batting average and strike-rate comparisons
- Centuries and fifties
- Fours and sixes
- Team-wise cumulative runs
- Season-wise average strike rate
- Runs versus strike rate
- Player consistency and outlier analysis

## ▶️ How to Run

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy requests beautifulsoup4 matplotlib scikit-learn jupyter
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `IPL_Batting_Web_Scraping.ipynb` and run the cells in order.

**Note:** The scraping code depends on ESPNcricinfo's page structure and availability, which may change over time. If the source blocks requests or changes its HTML, the scraper may need updates.

## ⚠️ Limitations

- This project focuses on batting statistics, not bowling or ball-by-ball analysis.
- Median imputation can influence averages, totals, and correlations.
- Player-season records are not the same as match-level records.
- Correlation does not establish causation.

## 👨‍💻 Author

**Varun Kumar**

- GitHub: [varun1181](https://github.com/varun1181)
- LinkedIn: [Varun Kumar](https://linkedin.com/in/varun-kumar-14t)

---

⭐ If you find this project useful, feel free to explore the notebook and share feedback.
