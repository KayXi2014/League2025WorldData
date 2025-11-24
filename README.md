# League2025WorldData
A curated dataset and tools for exploring League of Legends World Championship (Worlds) 2025 data — matches, teams, players, statistics and metadata. This repository collects cleaned historical and 2025-specific Worlds data intended for analysis, visualization, model-building, and reproducible research.

## Repository structure
- data
  - raw
    - Worlds 2025 Main Event - Champion Stats - OraclesElixir
    - Worlds 2025 Main Event - Team Stats - OraclesElixir
    - Worlds 2025 Main Event - Player Stats - OraclesElixir
  - processed
    - lol_matches_expanded
    - champion_clusters_analysis
- notebooks/             — Jupyter notebooks with example analyses and visualizations
  - champion_study.ipynb: contains Clustering Analysis for all champions used in World main stage
  - match_study.ipynb: contains Statistical Analysis for champion synergy and counter
- README.md              — this file
- Results
  - Results_Champion_Clustering
  - Results_Match_Analysis

## Data description
Sources
- Raw data downloaded from OraclesElixir(https://oracleselixir.com/stats/champions/byTournament/2025%20Season%20World%20Championship%2FPlay-In)
- Match data scraped from lol fandom(https://lol.fandom.com/Special:RunQuery/MatchHistoryGame?MHG%5Bpreload%5D=Tournament&MHG%5Bspl%5D=yes&MHG%5Btournament%5D=2025%20Season%20World%20Championship/Main%20Event&_run=) using code "match_scraper"

