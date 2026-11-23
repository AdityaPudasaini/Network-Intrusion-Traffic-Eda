# Network Intrusion Traffic: Exploratory Data Analysis

An end-to-end data preparation, statistical profiling, and visualization project analyzing over 488,000 network flow records (`ids.csv`) to compare **Normal Traffic** against **Infiltration Attacks**.

## Key Steps & Findings
* **Data Cleaning:** Filtered 79 network features down to 16 core flow metrics, removed missing values, and identified duplicate records.
* **Feature Correlation:** Discovered strong positive correlations (`> 0.94`) between packet counts, packet length means, and backward packet lengths.
* **Class Distribution:** Analyzed class balance between Normal Traffic and Infiltration Attacks.
* **Hypothesis Testing:** Performed an independent two-sample Welch's t-test on `Flow Duration` across traffic types ($p = 0.474$), indicating no statistically significant difference in mean flow duration alone.

## Tech Stack
* **Python**
* **Pandas** (Data manipulation & aggregation)
* **Matplotlib & Seaborn** (Heatmaps, bar charts, pie charts, and boxplots)
* **SciPy** (Statistical hypothesis testing)
