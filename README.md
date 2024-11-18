# A/B Testing for Marketing Campaign Effectiveness
### Author: Virendrasinh Chavda

<p align="justify">
This repository contains the code and analysis for evaluating the impact of two marketing campaigns (Ad and PSA) on conversion rates using <strong>A/B testing</strong>. The project employs statistical tests such as the Chi-Square Test, Point-Biserial Correlation, and Linear Regression to measure differences in conversion rates and assess the effect of ad frequency on conversions. 
</p>

## Table of Contents
1. [Overview](#Overview)
2. [Data](#Data)
3. [Methodology](#Methodology)
4. [Results](#Results)
5. [Future Work](#Future-Work)
6. [Contributing](#Contributing)
7. [License](#License)

## Overview
<p align="justify">
Money laundering is a sophisticated financial crime where illicit funds are disguised as legitimate. Traditional rule-based detection methods struggle with evolving and complex laundering schemes. In this project, we use <strong>network analysis</strong> techniques to detect money laundering by identifying central and suspicious nodes (accounts) in transaction networks. Centrality measures like <strong>degree</strong>, <strong>closeness</strong>, and <strong>betweenness centrality</strong> help uncover significant nodes. Additionally, community detection algorithms such as the <strong>Girvan-Newman algorithm</strong> are employed to isolate suspicious clusters of accounts.
</p>

<p align="justify">
Marketing campaigns are integral to driving customer engagement and conversions. In this project, we analyze A/B testing data to determine if different campaign strategies; Ad vs. PSA, significantly impact conversion rates. Using statistical tests, we assess if campaign type and ad frequency correlate with higher conversions and measure the practical impact of these factors on conversion likelihood. 
</p>

## Data:
The dataset used for this project includes anonymized user data on ad exposure and conversion outcomes, with the following key attributes:

* <strong>test group</strong>: Indicates the campaign type (`ad` or `psa`)
* <strong>converted</strong>: Binary variable indicating conversion (True/False)
* <strong>total ads</strong>: Number of ads shown to each user
* <strong>most ads day</strong>: Day of the week with the highest ad exposure
* <strong>most ads hour</strong>: Hour of the day with the highest ad exposure

<p align="justify">
For the purposes of this project, a subset of 2000 transactions was sampled and used for analysis due to computational constraints. Columns related to transaction type, timestamp, and fraud labels were excluded, focusing on <strong>network properties</strong>.
</p>

## Methodology:
### 1. Preprocessing
<p align="justify">
The dataset was cleaned by removing irrelevant columns and focusing on metrics essential for A/B testing, such as `test group`, `converted`, `total ads`, `most ads day`, and `most ads hour`.
</p>

### 2. Statistical Testing
The following statistical tests were conducted:
* <strong>Chi-Square Test</strong>: To compare conversion rates between `ad` and `psa` groups.
* <strong>Point-Biserial Correlation</strong>: To measure the association between `total ads` and conversion.
* <strong>Linear Regression</strong>: To estimate the effect of `total ads` on conversion probability.
* <strong>Effect Size Calculation (Cohen’s d)</strong>: To determine the practical significance of ad exposure differences between groups.

### 3. Visualization
Visualizations included:
* <strong>Conversion Rate by Day and Hour</strong>: Stacked bar plots for weekly and hourly conversion trends.
* <strong>Conversion vs. Total Ads</strong>: Scatter and box plots to visualize ad exposure differences by conversion status.

## Results:
* <strong>Conversion Differences</strong>: The Chi-Square test indicated significant conversion differences between the `ad` and `psa` groups.
* <strong>Ad Frequency Impact</strong>: A positive correlation between `total ads` and conversion probability was found, with regression results showing a small but significant increase in conversion with ad frequency.
* <strong>Effect Size</strong>: Cohen’s d showed an extremely small practical effect, indicating that while statistically significant, the difference in ad exposure is practically minimal. 


## Future Work:
* <strong>Incorporate Additional Features</strong>: Adding data on user demographics and behavior could refine insights.
* <strong>Longitudinal Analysis</strong>: Analyzing conversion trends over time may reveal seasonality or time-sensitive patterns.
* <strong>Machine Learning Integration</strong>: Building predictive models using these results could enhance campaign targeting and optimization. 

## Contributing
<p align="justify">
Contributions are welcome! If you would like to suggest improvements, report issues, or contribute to the project, feel free to open a pull request or submit an issue.
</p>

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

For more details, please refer to the [project report](https://github.com/VirendraChavda/Marketing-Effectivenes/blob/main/A_B%20Testing.ipynb).
