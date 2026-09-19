# Pakistan Cricket Intelligence & Global Player Analytics Platform

A reproducible sports data platform that automatically collects, validates, transforms, stores, and analyzes Pakistan cricket data — including the global/overseas careers of Pakistani players.

This is not just a Power BI dashboard. It's an end-to-end system: automated ETL → data warehouse → analytics → BI dashboard + API.

## 🚀 Live Dashboard
🔗 Coming soon (Power BI Publish to Web link)

## 📦 Project Structure

```
pak-cricket-intelligence/
├── etl/                  # Data Engineering: extract, clean, validate, load
│   ├── extractors/
│   ├── transformers/
│   └── loaders/
├── database/
│   └── schema/           # Star schema (dim/fact tables)
├── analysis/              # EDA notebooks, data analysis write-ups
├── models/                # Data Science models
│   ├── training/
│   └── evaluation/
├── dashboard/
│   └── pbix/               # Power BI file
├── api/                     # FastAPI backend
├── tests/                   # pytest test suite
├── docs/
│   └── screenshots/         # Dashboard screenshots/GIFs
└── README.md
```

## 🧩 Modules

- Executive Overview
- Match Center
- Player Intelligence (Career, Form, Matchups, Phase Analysis, Venue Performance, Home/Away, Global Career)
- Pakistan Teams (Men's, Women's, U19, Domestic)
- Global Pakistani Players (Leagues, Countries, Teams, Overseas Statistics)
- Tournaments
- Matchup Engine
- Team Intelligence
- Venue Intelligence
- Records & History
- Player Similarity
- Player Value Model
- Automated Insights
- Data Engineering (ETL Status, Data Quality, Data Lineage, Pipeline Monitoring)

## 🛠️ Tech Stack

**Core:** Python, Pandas, SQL, PostgreSQL, Power BI, Git/GitHub
**Engineering:** dbt, Docker, GitHub Actions, pytest, Pandera, FastAPI
**Data Science:** scikit-learn, statsmodels/Prophet

## 🗄️ Data Architecture

```
Official/permitted sources → Extractors → Raw/Staging → Cleaning → Validation
→ PostgreSQL → dbt → Analytical Models → Power BI / FastAPI
```

## 📊 Data Model

Star schema: `dim_player`, `dim_team`, `dim_venue`, `dim_tournament`, `dim_date`, `dim_format` → `fact_match` (batting/bowling/fielding)

Plus operational tables: ETL runs, data sources, rejected records, pipeline watermarks, data-quality results.

## ✅ Status

🚧 In Progress — Project setup phase

## 📥 Setup

```bash
git clone https://github.com/mwaleedn12-pixel/pak-cricket-intelligence.git
cd pak-cricket-intelligence
```
*(Full setup instructions will be added as ETL and database modules are built)*