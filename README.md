# NFL Quarterback GOAT Analytical Model

[![Google Sheets](https://img.shields.io/badge/Google_Sheets-View_Live_Model-success?style=for-the-badge&logo=googlesheets)](https://docs.google.com/spreadsheets/d/1wCGeV-194F5a9CaFOrZiJQmLf2ba2pUVidcrwqGBIYE/edit?usp=sharing)

## Project Overview

A data-driven framework for evaluating the greatest quarterbacks in NFL history using **era-adjusted statistics, normalization techniques, and multi-model scoring**.

Rather than relying on a single metric or subjective ranking, this project builds four separate analytical models that evaluate different dimensions of quarterback performance. The models are combined into a final **GOAT Score** to produce a comparative ranking across eras.

Because NFL passing environments have changed dramatically over time, the analysis uses **era adjustment and z-score normalization** to compare players relative to their contemporaries rather than raw totals.

---

## Technical Methodology

The core challenge of this project was comparing quarterbacks from the modern passing era to those of earlier eras. To solve this, the model utilizes a **Relative Value Framework**:

* **Era-Adjustment (Relative to Mean):** Each season's statistics are compared against the league average for that specific year. This ensures that a 4,000-yard season in 1980 is weighted appropriately compared to a 4,000-yard season in 2024.
* **Z-Score Normalization:** Every metric is converted into a z-score, representing how many standard deviations a player sits above or below the era mean. This allows "Greatness" (awards) to be mathematically combined with "Efficiency" (ANY/A).
* **Weighted Aggregation:** The final **GOAT Score** is a composite index. Each of the four pillars (Greatness, Best, Dominant, Clutch) is assigned a specific percentage weight based on historical significance and data reliability.

---

## Spreadsheet Architecture

The workbook is engineered for scalability and clarity, following a three-tier software-style structure:

1.  **Presentation Layer:** `DASHBOARD` and `FINAL_GOAT_RANKINGS`. These utilize data validation and conditional formatting for high-level insights.
2.  **Calculation Layer:** Hidden sheets that handle the z-score math, weighting distributions, and era-lookup tables.
3.  **Data Layer:** `DATA_QB_SEASONS` and `DATA_AVG_SEASONS`, acting as the "Source of Truth" for the model.

---

## The Four-Pillar Model

The model evaluates quarterbacks through four analytical lenses:

**Greatest**
Measures career legacy and accomplishments, including major awards, championships, and long-term achievements.

**Best**
Evaluates overall performance level using efficiency metrics such as **ANY/A+ (Adjusted Net Yards per Attempt relative to league average)**.

**Dominant**
Measures how much a quarterback separated himself from league averages during his career using season-level statistical comparisons.

**Clutch**
Analyzes postseason performance and whether quarterbacks elevated their play in playoff situations.

Each pillar produces an independent ranking, which are then combined into a final composite **GOAT Score**.

---

## Dataset

The model evaluates **25 historically significant NFL quarterbacks** spanning multiple eras of professional football. I relied on [Pro Football Reference](https://www.pro-football-reference.com/) and [StatMuse](https://www.statmuse.com/) for data collection.

The dataset includes:

* career statistical totals
* season-by-season quarterback performance
* league averages by season

These inputs allow the model to construct **era-adjusted and relative performance metrics**.

---

## Skills Demonstrated

This project was designed as a portfolio example of applied data analysis using spreadsheet tools.

**Statistical Modeling**

* Z-score normalization
* Weighted scoring models
* Era-adjusted statistical comparisons

**Advanced Spreadsheet Techniques**

* Multi-sheet analytical architecture
* XLOOKUP and conditional logic
* Data normalization workflows

**Data Presentation**

* Interactive dashboard design
* Visual ranking comparisons
* Structured analytical reporting

---

## Workbook Structure

The spreadsheet is organized into several layers:

**Presentation Layer**

* Dashboard
* Final Rankings
* Quarterback Roster

**Model Layer**

* Greatest Model
* Best Model
* Dominant Model
* Clutch Model

**Calculation Layer**

Hidden sheets contain the underlying normalization calculations, raw data tables, and intermediate metrics used to construct the models.

---

## How to Explore the Project

1. Start with the **Dashboard** sheet for a visual overview of the rankings.
2. Review the **Model Results** sheet to see how quarterbacks rank across each analytical model.
3. Explore individual model sheets to understand how scores are calculated.

