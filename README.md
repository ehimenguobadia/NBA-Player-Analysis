# NBA Draft Analysis (1989–2021)

A short data analysis exploring the relationship between NBA draft position and long-term career scoring, using draft classes from 1989 through 2021.

## Research Question

Which players from each draft class went on to score the most career points, and is there a relationship between where a player was drafted and how much they scored over their career?

## Files

- `nba_analysis.qmd` — Quarto source file with the full analysis (code + writeup)
- `nba_analysis.html` — Rendered report
- `nbaplayersdraft.csv` — Dataset used in the analysis

## Data

The dataset contains one row per drafted player (1989–2021) with fields including draft year, overall pick, team, career games/points/rebounds/assists, shooting percentages, and advanced metrics like win shares and box plus-minus.

## Methods

The data was cleaned to remove missing values and narrowed to the relevant variables. Summary statistics and three visualizations (histogram, scatterplot, bar chart) were used to explore the distribution of career points and its relationship to draft position.

## Requirements

- [R](https://www.r-project.org/) (4.x+)
- [Quarto](https://quarto.org/)
- R packages: `tidyverse`

## Running the Analysis

```bash
git clone <your-repo-url>
cd <repo-folder>
quarto render nba_analysis.qmd
```

This regenerates `nba_analysis.html` from the source `.qmd` and CSV.

## Key Findings

- A small number of elite players account for a disproportionate share of career scoring; most drafted players score relatively few career points.
- Earlier draft picks tend to score more career points on average, though there are notable exceptions.
- Apparent scoring trends in recent draft classes are affected by survivorship/recency bias — many recently drafted players are still early in their careers.

## Limitations

This analysis considers total career points only. It doesn't account for career length, injuries, playing time, or other performance metrics (rebounds, assists, steals, blocks). Future work could incorporate these factors for a fuller picture of scoring success.

## Contributors

This was a group project — contributions have been anonymized for the public repo.
