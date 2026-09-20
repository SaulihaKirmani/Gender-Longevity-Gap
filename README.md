# Do Women Live Longer Than Men? A Global Demographic Study

An empirical, spatial, and inferential analysis investigating the global female longevity advantage using World Bank API data and R/Quarto.

## Key Features & Findings
- **Data Pipeline:** Ingested live World Bank indicators (`SP.DYN.LE00.FE.IN`, `SP.DYN.LE00.MA.IN`, `NY.GDP.PCAP.CD`) via `wbstats`.
- **Inferential Testing:** Evaluated normality (Shapiro-Wilk) and confirmed a statistically significant global female longevity advantage via dual testing (Paired $t$-test & Wilcoxon Signed-Rank, $p < 0.001$).
- **Income Stratification:** Assessed cross-tier heterogeneity across 4 World Bank income levels using Kruskal-Wallis non-parametric testing.
- **Boundary Outlier Analysis:** Identified upper and lower tail extremes (Tukey's 1.5*IQR) and highlighted socio-economic cross-tier anomalies (Central African Republic in the upper tail; Kuwait, Bahrain, and Qatar in the lower tail).

## Tech Stack
- **Language:** R
- **Publishing Engine:** Quarto (`.qmd`)
- **Key Libraries:** `tidyverse`, `wbstats`, `ggrepel`, `plotly`, `knitr`
