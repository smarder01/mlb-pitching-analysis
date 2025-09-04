# MLB Pitching Analytics: Advanced Metrics and Trends (2000-2024)

## Overview
This project analyzes MLB pitching performance from 200-2024 using the Lahman database.

The workflow demonstatres a complete analytics pipeline:
- Data cleaning and feature engineering (Python)
- Database integration and SQL practice (SQLite & DB Browser)
- Exploratory analysis and visualization (Python & Tableau)

The goal is to evaluate pitcher performance using modern sabermetric indicators such as K/9, BB/9, HR/9, and WHIP, while also showcasing reproducible data science skills.

---

## Project Structure
mlb-pitching-analytics/
│
├── data/
│   ├── lahman_data/             # Raw Lahman database CSVs
│   ├── cleaned_data/            # Processed datasets (e.g, pitching_clean.csv)
│       ├──  pitching_clean.csv
│       └── pitching_tableay.csv
│   └── baseball.db/
│
├── notebooks/
│   └── pitching_analysis.ipynb  # Main analysis notebook
│
├── tableau/
│   └── Baseball_Pitching_Dashboard_2024.twbx  # Tableau dashboard (packaged workbook)
│
├── visuals/
│   ├── example_k9.png           
│   ├── example_k9.png   
│   └── example_k9.png   
│
├── README.md                    # Project documentation
└── requirements.txt             # Python dependencies (optional)

---

## Project Highlights

- Data Cleaning → Filtered modern-era pitchers (2000–2024, ≥30 IP) and converted raw stats (IPouts → innings).
- Feature Engineering → Created advanced metrics: K/9, BB/9, HR/9, WHIP.
SQL Integration → Loaded data into SQLite, practiced queries in Python and DB Browser.
- Exploratory Analysis → Visualized strikeout trends, WHIP distributions, and top pitchers.
- Tableau Dashboard → Built an interactive dashboard for filtering by year, pitcher, and team.

---

## Visuals

**1. League-Average Strikeouts and Walks Over Time (k9_vs_bb9.png)**
This visualization shows how pitching has evolved since 2000. Strikeouts per 9 innings (K/9) have risen steadily, reflecting the modern emphasis on power pitching, while walks per 9 innings (BB/9) have remained relatively stable.
<img width="2532" height="1634" alt="k9_vs_bb9" src="https://github.com/user-attachments/assets/ce5e7689-a2da-485b-a80d-dc2608b22fb5" />

**2. ERA Distribution by Season (era_by_season.png)**
This plot highlights how run prevention has varied across MLB seasons. Shifts in the distribution of ERA values illustrate how factors like the juiced ball era, pitching changes, and league-wide strategies have influenced pitcher performance.
<img width="3000" height="1800" alt="era_by_season" src="https://github.com/user-attachments/assets/1dd44056-a692-4051-b195-e99f5779cf07" />

**3. WHIP Comparison Across Pitchers (whip_dist.png)**
This chart compares pitcher efficiency using WHIP (walks + hits per inning pitched). Lower WHIP values indicate better ability to limit baserunners, making it a strong measure of pitcher dominance.
<img width="2111" height="1403" alt="whip_dist" src="https://github.com/user-attachments/assets/55175db7-5f90-4ebb-9fba-c87990716c65" />

---

## Tableau Dashboard

This project includes an interactive Tableau dashboard that highlights both individual pitcher performance and team-level comparisons.

**Key Features:**
- Top K/9 Pitchers (2024) → Identifies the highest strikeout pitchers of the season.
- ERA Leaders Over Time → Tracks league ERA trends from 2010–2024, showing how pitching dominance has shifted.
- Team Pitching Leaderboard (2024) → Compares teams across ERA, WHIP, K/9, BB/9, and HR/9.
- Team WHIP Rankings (2024) → Highlights team efficiency in limiting baserunners.

You can explore the interactive dashboard here:  
[View on Tableau Public](https://public.tableau.com/shared/XJNQZBTDR?:display_count=n&:origin=viz_share_link)

---

## Future Directions

Currently, this project emphasizes pitching performance trends and player/team comparisons. Moving forward, I plan to extend the analysis to include:

- **Batting**: Metrics like OPS, wOBA, and home run rates.
- **Fielding**: Defensive efficiency, errors, and advanced fielding stats.
- **Filters by Team/Season**: Interactive dashboards where users can choose a team and see a complete breakdown of pitching, hitting, and fielding.
- **Deeper Advanced Analytics**: Incorporating sabermetrics (e.g., WAR, FIP, wRC+) for a more advanced evaluation.

This will transform the project from a pitching-focused study into a full baseball analytics platform.
