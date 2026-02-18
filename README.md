UK Crime Analysis: Temporal, Spatial & Statistical Investigation of Violent and Firearm Offences

## Problem Statement

Public discourse often raises critical questions about crime in the UK:

* Are violent crimes increasing, decreasing, or remaining stable over time?
* Does Liverpool have the highest per capita firearm incident rate compared to other regions?
* Is there a measurable association between firearm-related and drug-related offences?

While open crime datasets are publicly available, raw data alone does not answer these claims. The challenge lies in transforming large, heterogeneous crime records into structured insights using scalable data processing and rigorous statistical analysis.

This project addresses that challenge through a structured, data-driven investigation of UK crime patterns.

---

## Why This Solution?

Crime data is:

* Large-scale and multi-dimensional
* Geographically distributed
* Temporally continuous
* Statistically noisy

To properly evaluate the claims, a simple descriptive analysis would not be sufficient. Instead, this project proposes a **multi-layered analytical framework** combining:

* Big data processing (Apache Spark)
* Time-series trend analysis
* Per capita normalization
* Correlation and statistical evaluation
* Spatial visualization

This approach ensures that conclusions are evidence-based rather than assumption-driven.

---

## Technical Approach

### 1️⃣ Scalable Data Processing

Given the size of UK crime datasets, the project uses **Apache Spark (PySpark)** to:

* Load structured crime data efficiently
* Define explicit schemas
* Perform distributed filtering and aggregation
* Maintain computational scalability

Data cleaning and preprocessing steps include:

* Handling missing values
* Filtering relevant offence categories
* Structuring temporal fields for time-series analysis

---

### 2️⃣ Time-Series Analysis of Violent Crime

To evaluate whether violent crime trends are increasing or decreasing:

* Crimes were aggregated over time
* Line plots and rolling means were used to smooth variability
* Linear regression was applied to quantify trend direction

Rather than relying on visual interpretation alone, the slope of the regression model provides measurable evidence of trend behavior.

---

### 3️⃣ Per Capita Firearm Incident Comparison

Raw crime counts can be misleading due to population differences.

To address this:

* Firearm incidents were normalized using regional population data
* Per capita rates were calculated
* Comparative analysis was conducted across selected regions, including Liverpool

This ensures fair cross-regional comparison and avoids statistical bias.

---

### 4️⃣ Correlation Between Firearm and Drug Offences

To investigate potential associations:

* Offence categories were aggregated by geography
* Correlation matrices were computed
* Statistical measures were used to assess strength and direction of relationships

This allows us to move beyond anecdotal claims and quantify whether firearm and drug-related crimes exhibit spatial or statistical co-occurrence.

---

### 5️⃣ Visualization & Spatial Context

Multiple visualization techniques were used to strengthen interpretability:

* Time-series line plots
* Rolling averages
* Correlation heatmaps
* Geographical mapping (Cartopy-based spatial representation)

Each visualization method was selected to match the analytical objective — temporal trends, regional comparisons, or relational insights.

---

## Evaluation & Reasoning

The proposed analytical framework was chosen because:

* Time-series modeling provides objective trend measurement
* Per capita normalization ensures equitable comparison
* Correlation analysis quantifies inter-offence relationships
* Spatial visualization adds geographical context

This layered approach increases analytical robustness and reduces the risk of misleading conclusions.

---

## Outcome

By combining distributed data processing, statistical modeling, and visual analytics, this project transforms open crime datasets into structured insights that can inform:

* Policy evaluation
* Law enforcement resource allocation
* Evidence-based public safety discussions

Rather than treating crime data as static records, this project demonstrates how data science can uncover meaningful patterns across time, space, and offence categories.


