# Group7---Phase-2

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

## 📊 Dataset Description
The dataset is compiled from publicly available and industry-recognized sources:

- **Box Office Mojo** – Domestic and foreign box office revenue  
- **IMDb** – User ratings and vote counts  
- **Rotten Tomatoes** – Critical reception  
- **The Movie Database (TMDb)** – Popularity scores, genres, and metadata  

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

Foreign revenue > Domestic revenue

Revenue success is not evenly distributed

The industry is hit-driven, especially in the domestic market

Blockbusters generate massive ROI compared to low- and mid-tier films

Average metrics (means) are misleading due to extreme skewness

## Strategic Implications for a New Studio

From a studio strategy perspective:

Profitability depends on rare breakout hits

Risk is concentrated, not evenly spread

Decisions based purely on average revenue are unreliable

## Recommendations

To compete effectively while managing risk, a new studio should:

Focus on high-impact, globally appealing films

Prioritize sequels, franchises, and proven genres

Target international markets early

Use median and percentile-based metrics rather than averages

Avoid over-investing in low-tier films without breakout potential

## Repository Structure
├── data/                # Raw and cleaned datasets
├── film_performance.ipynb    # Jupyter notebooks for analysis
├── visuals/             # Generated charts and plots
├── src/                 # Supporting scripts
└── README.md            # Project documentation
|__ .gitignore

### Final Note

This analysis demonstrates that success in the modern film industry is driven by strategic risk-taking, global appeal, and data-informed decision-making, rather than volume-based production or reliance on average performance indicators.
