# PSP Sales Factorial Analysis

A two-way factorial analysis of Sony PSP game sales, examining the effects of game genre and release period on global sales. Utilizes exploratory visualization, ANOVA, and post-hoc analysis to uncover market trends in the portable gaming ecosystem.

---

## Table of Contents

- [Project Overview](#project-overview)  
- [Dataset](#dataset)  
- [Research Question](#research-question)  
- [Experimental Design](#experimental-design)  
- [Analysis Methods](#analysis-methods)  
- [Results](#results)  
- [Conclusions & Insights](#conclusions--insights)  
- [Reproducibility](#reproducibility)  
- [Project Structure](#project-structure)  
- [Contributors](#contributors)  
- [License](#license)  

---

## Project Overview

This study investigates how video game **genre** (Action, Adventure, Role-Playing, Strategy) and **release period** (Early: 2004–2007, Mid: 2008–2011, Late: 2012–2015) influence global sales in the PlayStation Portable (PSP) market. Applying a replicated two-way factorial design and ANOVA, we quantify main effects and explore interaction patterns.

---

## Dataset

- **Source:** Proprietary compilation of PSP game sales  
- **Observations:** 679 games  
- **Factors:**  
  - **Genre:** Action, Adventure, Role-Playing, Strategy  
  - **Time Period:** Early, Mid, Late  
- **Response:** Global sales (millions of units)

---

## Research Question

> How do game genre and release timing affect commercial success in the PSP market, and is there an interaction between these factors?

---

## Experimental Design

- **Design Type:** 4×3 factorial (4 genres × 3 time periods)  
- **Replication:** Multiple titles within each cell (n varies cell-wise)  
- **Balanced Analysis:** ANOVA with diagnostic checks for normality and homogeneity  

---

## Analysis Methods

1. **Data Visualization**  
   - Boxplots of sales by genre and period  
2. **Assumption Validation**  
   - Shapiro-Wilk test (normality)  
   - Levene’s test (homogeneity)  
3. **Two-way ANOVA**  
   - Main effects of Genre and Period  
   - Interaction term  
4. **Effect Estimates**  
   - Factor level contrasts with 95% confidence intervals  
5. **Interaction Plots**  
   - Visual assessment of genre trends across periods

---

## Results

- **ANOVA Findings:**  
  - **Genre:** Significant effect on sales (p < 0.001)  
  - **Time Period:** Significant effect on sales (p < 0.001)  
  - **Interaction:** Not significant (p = 0.292)  
- **Main Effects:**  
  - Action (+0.093) and Role-Playing (+0.061) outperformed baseline  
  - Adventure underperformed (−0.145)  
  - Early period strong positive effect (+0.158), Late period decline (−0.135)  

---

## Conclusions & Insights

- **Genre Impact:** Action and RPG titles consistently drove higher sales; Adventure titles lagged.  
- **Lifecycle Effect:** Strong launch-period performance, followed by gradual decline.  
- **Market Strategy:** Focus on Action/RPG for robust sales; consider timing to maximize launch impact.  

---

## Reproducibility

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/psp-sales-factorial.git
   cd psp-sales-factorial
   ```

2. **Install R dependencies**  
   ```r
   install.packages(c("tidyverse", "car", "ggplot2", "rmarkdown"))
   ```

3. **Render the analysis**  
   ```r
   rmarkdown::render("STA305 Assignment 4.Rmd")
   ```

4. **Review outputs**  
   - `STA305 Assignment 4.html` for interactive report  
   - `STA305 Assignment 4.pdf` for formatted document

---

## Project Structure

```
├── STA305 Assignment 4.Rmd     # R Markdown analysis  
├── STA305 Assignment 4.pdf     # Final report  
├── data/                       # Raw and processed data files  
├── figures/                    # Plots and diagnostic charts  
└── README.md                   # This file  
```

---

## Contributors

- **Mohammad Danish Malik** – Design, analysis, interpretation, writing  

---

## License

Released under the MIT License. See [LICENSE](LICENSE) for details.
