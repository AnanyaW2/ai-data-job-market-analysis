# AI & Data Job Market Analysis (2025–2026)

An end-to-end data analysis project exploring 1,500 real AI and data job postings — which skills pay the most, how AI-native roles compare to traditional ones, where the highest-paying markets are, and where hiring demand is heading next.

**Live interactive dashboard:** [Tableau Public link] ← replace with your published link
**Portfolio write-up:** [Your portfolio site link] ← replace with your site link

---

## Overview

This project analyzes a dataset of 1,500 AI/ML job postings covering 25 distinct roles across 14 countries — including emerging titles like LLM Engineer, RAG Engineer, and AI Agent Developer that don't appear in older job-market datasets. The goal was to answer a practical question: **if you're job-hunting in AI/data right now, where should you actually focus?**

## Key Findings

1. **RAG, Prompt Engineering, and LLM Fine-tuning lead on both pay and growth.** These skills rank among the highest-paying in the dataset (avg. $240K+) while also showing some of the fastest year-over-year demand growth.

2. **The AI-native salary premium is earned, not automatic.** At entry level, AI-native and traditional roles pay almost identically (~$151K vs. ~$150K). The gap widens sharply with seniority, reaching roughly 11% by the Lead level (~$258K vs. ~$235K).

3. **Remote-friendliness varies widely by country.** Singapore leads at 43.7% fully-remote AI/data postings; Germany trails at 21.0%.

4. **Roles cluster into two distinct groups, with a gap between them.** Established roles (Data Scientist, ML Engineer) show steady ~15–20% YoY growth. Emerging AI-native roles (LLM Engineer, RAG Engineer) show ~45–55% YoY growth — almost nothing falls in between.

## Data

- **Source:** [AI Jobs Market 2025-2026 dataset, Kaggle](https://www.kaggle.com/datasets/alitaqishah/ai-jobs-market-2025-2026-salaries)
- **Size:** 1,500 rows, 25 columns
- **Coverage:** 25 job titles, 14 countries, Oct 2025–2026 postings

## Process

1. **Exploratory analysis (Python / pandas):** checked data types, nulls, and distributions; parsed a pipe-delimited `required_skills` field into a long-format table to analyze skill-level salary and demand trends (`skill.explode()` pattern).
2. **Analysis questions:** defined upfront — skill-to-salary relationships, AI-native vs. traditional role comparisons by experience level, geographic patterns, and a demand-vs-growth view to identify where the market is heading.
3. **Dashboard build (Tableau Public):** four connected views — Overview, AI-Native vs. Traditional Roles, Geography, and Demand vs. Growth — iterating on chart choice along the way (e.g., replacing a hard-to-read 100%-stacked bar with clean grouped bars after review, to prioritize clarity over density).

## Repository Contents

| File | Description |
|---|---|
| `analysis.ipynb` | Python notebook — data cleaning, exploration, skills-parsing logic |
| `ai_data_job_market.twbx` | Tableau packaged workbook (all 4 dashboards) |
| `ai_jobs_market_2025_2026.csv` | Raw dataset |

## Tools

Python (pandas) · Jupyter · Tableau Public

---

*Part of a broader portfolio spanning analytics/BI, data science/ML, and applied AI projects — see [portfolio site link].*
