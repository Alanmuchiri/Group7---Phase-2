# Group7 Phase-2 Project

# 🎬 Movie Industry Statistical Analysis  
## Studio Strategy & Risk-Aware Market Entry

---

##  Project Overview
This project presents a statistical and exploratory analysis of the global film industry to support strategic decision-making for launching a **new movie studio**. The analysis focuses on understanding revenue concentration, audience preferences, and financial risk in a market dominated by established studios with strong franchises, large marketing budgets, and global distribution power.

---

##  Business Objective
The company aims to venture into **original video creation** by establishing a new movie studio.  
The goal of this analysis is to determine:

- What types of films align with current audience demand  
- How revenue is distributed across domestic and foreign markets  
- How financial risk can be minimized while remaining competitive  
- Why relying solely on average performance metrics can be misleading  

---

### Dataset Descriptions

- **`bom.movie_gross.csv`**  
  Box Office Mojo data containing domestic, foreign, and worldwide gross revenue.

- **`tmdb.movies_cleaned.csv`**  
  TMDb movie metadata including popularity scores, genres, languages, and audience ratings.

- **`tn.movie_budgets.csv`**  
  Production budgets and revenue figures used for return on investment (ROI) analysis.

- **`IMDb Database`**  
  Intended for use via SQLite for extended ratings and vote-level analysis.
 

These platforms aggregate data from industry reports, critics, and user contributions, making the dataset suitable for analyzing relationships between **movie characteristics, reception, and commercial performance**.

---

## Tools & Libraries Used
The analysis and visualizations were performed using Python and the following libraries:

```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
from scipy.stats import skew, kurtosis, norm
import ast
import _sqlite3
```

##  Tableau Dashboard

In addition to Python-based visualizations using Matplotlib and Seaborn, an interactive Tableau dashboard was created to enhance exploratory analysis and stakeholder communication.

The Tableau dashboard was used to:
- Compare domestic vs foreign revenue distributions
- Visualize ROI concentration and blockbuster impact
- Explore genre performance across revenue and popularity
- Identify skewness and outliers through interactive filtering

This allowed non-technical stakeholders to explore trends dynamically and validate statistical findings derived from Python analysis.

Below is a link to the various sheets , the dashboard and the story in tableau public :
* [https://public.tableau.com/app/profile/layla.isse5307/viz/Film_Performance/TotalNetGrossbyStudioTopStudios](https://public.tableau.com/views/Film_Performance/MovieProfitabilityWhatDrivesFinancialSuccess?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Key Statistical Findings
### Revenue Distribution

Foreign revenue dominates the film industry, exceeding domestic revenue in most cases.

Most movies earn below 50 million USD in total revenue.

The highest concentration of domestic gross lies between 0–10 million USD.

A small number of films generate extremely high returns, heavily influencing totals.

Return on Investment (ROI)

Average ROI is approximately 50,000%, driven by a small number of blockbusters.

Blockbuster films achieve disproportionately higher ROI compared to low-tier releases.

### Skewness Analysis

All major revenue variables are strongly right-skewed, indicating:

Most movies earn low to moderate revenue

A small number of films earn exceptionally high revenue

The long right tail is caused by blockbuster releases

Domestic revenue exhibits the highest skewness, suggesting it is more hit-driven than foreign revenue.

### Kurtosis Analysis

All revenue distributions show high kurtosis (fat tails)

Extreme values occur far more frequently than in a normal distribution

A small number of movies dominate total industry revenue

Domestic revenue shows the highest kurtosis, reinforcing the presence of extreme outliers.

### Audience & Popularity Insights

Average audience rating: ~6

Average popularity score: ~5

A limited number of movies exceed popularity scores of 7

High popularity does not guarantee high revenue, but blockbusters often combine both

### Genre Performance

The three most commercially successful and popular genres are:

Action

Adventure

Animation

These genres consistently perform well in both domestic and foreign markets.

## Key Conclusions

Revenue success is highly uneven
Movie revenues are heavily skewed, with a small number of films generating a disproportionate share of total industry returns.

The industry is hit-driven
Blockbuster films vastly outperform low- and mid-tier releases, particularly in the domestic market.

Foreign revenue dominates domestic revenue
International box office consistently exceeds domestic earnings and is the primary driver of overall profitability.

Release timing has a significant impact
Films released during summer and winter (holiday periods) tend to achieve higher profits compared to off-season releases.

Large budgets do not guarantee profitability
Higher production budgets increase financial risk and do not reliably result in higher returns.

Audience ratings offer limited differentiation
Most films cluster between ratings of 6–8 regardless of popularity or revenue performance.

Mass appeal is genre-driven
Action, adventure, and fantasy genres consistently dominate audience demand and revenue outcomes.

Average metrics are misleading
Mean revenue and profit figures are distorted by extreme outliers; median and percentile-based measures provide more reliable insights.

## Strategic Implications for a New Studio

Profitability depends on rare breakout hits, not steady moderate performance.

Financial risk is highly concentrated, rather than evenly distributed across projects.

Decisions based solely on average revenue metrics can lead to systematic capital misallocation.

While the movie market is structurally growing, strong performance depends on quality, genre selection, and release timing.

## Recommendations

Design films for the global market first
Prioritize international appeal in storytelling, casting, and distribution strategies.

Allocate resources to high-potential titles
Focus marketing and distribution efforts on films with clear blockbuster characteristics.

Exploit peak release windows
Reserve summer and holiday periods for high-budget, mass-appeal films; use off-season slots for lower-budget or experimental projects.

Adopt ROI-driven decision-making
Evaluate projects using expected ROI and percentile-based performance metrics rather than averages.

Build long-term franchises
Prioritize sequels and proven genres, treating successful films as long-term assets rather than one-off wins.

## Repository Structure
├── data/                * Raw and cleaned datasets
├── film_performance.ipynb    # Jupyter notebooks for analysis
├── visuals/             # Generated charts and plots
├── src/                 # Supporting scripts
└── README.md            # Project documentation
|__ .gitignore

### Final Note

This analysis demonstrates that success in the modern film industry is driven by strategic risk-taking, global appeal, and data-informed decision-making, rather than volume-based production or reliance on average performance indicators.
