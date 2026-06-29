# 🏏 IPL Data Analysis Project (2008 - 2025)

## 📌 Project Overview
This repository contains a comprehensive data analysis and visualization dashboard tracking the evolution of the Indian Premier League (IPL) from its inception in 2008 up to 2025. The project uncovers deep insights into team performance, batting and bowling metrics, and seasonal accolades like the Orange and Purple Cap holders. 

The core deliverable of this analysis is an interactive, data-driven dashboard, which allows users to dynamically filter statistics by season (e.g., exploring the 2018 season where Chennai Super Kings lifted the trophy).

---

## 📊 Dashboard Preview

![IPL Analysis Dashboard](image_bee2bd.jpg)

---

## 📁 Dataset Description

The analytical engine behind this dashboard is powered by combining four core relational datasets:

### 1. `ball_by_ball_data.csv`
* **What it is:** The granular, event-level backbone of the project, containing **278,205 individual ball deliveries**.
* **Key Fields Used:** `over_number`, `ball_number`, `batter_runs`, `extras`, `total_runs`, `is_wicket`, `is_wide_ball`, `is_no_ball`.
* **Analytical Purpose:** Used to calculate aggregate season-long boundary metrics (e.g., the **872 Sixes** and **1,652 Fours** hit in 2018), compute raw player runs for the Orange Cap race, and extract bowler wicket counts for the Purple Cap.

### 2. `ipl_matches_data.csv`
* **What it is:** The match-level metadata ledger tracking **1,169 total matches** played across IPL history.
* **Key Fields Used:** `match_id`, `season`, `venue`, `toss_winner`, `toss_decision`, `match_winner`, `win_by_runs`, `win_by_wickets`.
* **Analytical Purpose:** Crucial for constructing the dynamic **Points Table** (Games Played, Won, Lost, Points), finding seasonal counts (e.g., **60 matches** across **10 venues** in 2018), and determining the ultimate Champion and Runner Up per season.

### 3. `players-data-updated.csv`
* **What it is:** A comprehensive biographical roster of **772 IPL players**.
* **Key Fields Used:** `player_id`, `player_name`, `bat_style`, `bowl_style`, `player_image`.
* **Analytical Purpose:** Allowed for mapping player IDs to user-friendly player names (e.g., matching player metrics to showcase names like *KS Williamson* or *AJ Tye*) and classifying player styles.

### 4. `teams_data.csv`
* **What it is:** A lookup reference containing information on **16 distinct franchise teams** across the timeline.
* **Key Fields Used:** `team_id`, `team_name`, `team_name_short`, `image_url`.
* **Analytical Purpose:** Used for cleaning and mapping inconsistent historical team names (e.g., verifying teams active during specific years, like the 8 active teams in 2018) and pulling official branding assets.

---

## 💡 Core Insights & Features Present on Dashboard

* **Dynamic Seasonal Filtering:** Seamless slice-and-dice capability spanning nearly two decades of IPL history.
* **High-Level KPIs:** Instant snapshot of Total Sixes, Fours, Matches, Teams, Centuries, Half-Centuries, and Venues utilized per season.
* **Accolades Section:** Dedicated visuals spotlighting the individual standard-bearers of the tournament—the top run-scorers and leading wicket-takers.
* **Automated Standings Table:** An accurate, sorted league table calculating total team points and performance splits.

---

## 🛠️ Tech Stack & Tools Used
* **Data Cleaning & Preprocessing:** Python (Pandas) / Excel / Power Query
* **Data Modeling:** Star Schema / Relational Data Joins
* **Visualization:** Power BI / Tableau *(Change this to match your visualization tool)*
