# Cost-Optimization-Analysis-for-Eesti-Energia

Data analysis project developed as part of the Eesti Energia challenge, promoted by the **[Data Vinking](https://www.dataviking.com.br/)** data community. 

This document summarizes the trajectory of the data analysis project, highlighting the main points and visualizations.

The complete study is available clicking here, or by accessing the file Project.ipynb located in this repository.

Project developed by Lucas Pontes *[profile](https://www.linkedin.com/in/lucasdpontes/)*

<br><br><h1 align="center">Introduction</h1>

<p><img src="https://github.com/lucas-dpontes/Cost-Optimization-Analysis-for-Eesti-Energia/blob/main/eesti-logo.png"></p><br>

Eesti Energia (https://www.enefit.ee/en) is an energy company located in Estonia. It is the largest oil shale energy company in the world.

In 2014, it operated in Estonia, Latvia, Lithuania, Finland, Jordan, and Utah (United States).

The group has three main areas of operation:
- electricity generation
- oil shale production
- electricity sales and distribution

**Business Pain:** high production cost

**Root Cause:** high energy cost

**Main Goal:** study the energy cost data and suggest an action plan to reduce the cost

<br><br><h1 align="center">Analysis</h1>

## Annual average price

<div align="center">

| Month | Average price [€] |
|:-:|:-:|
| 2021 | 137.2 |
| 2022 | 192.8 |
| 2023 | 86.2 |

</div>

A peak period was observed in 2022, followed by a sharp decline in 2023. It is advisable to analyze these variations more deeply.

## Moving average of prices

<p align="center"><img src="https://github.com/lucas-dpontes/Cost-Optimization-Analysis-for-Eesti-Energia/blob/main/temporal-analysis.png"></p><br>

Based on the graph above, it can be observed that there is a significant variation in prices, with sharp peaks in 2022, followed by a gradual decline and stabilization in 2023.

The daily data (gray line) shows high fluctuations, while the weekly (blue line) and monthly (green line) averages smooth out the variations, highlighting long-term trends.

The observed peaks, particularly in 2022, may be linked to energy crises or external factors affecting the market, such as increased demand or supply restrictions.

From 2023 onwards, prices exhibit lower volatility and reduced levels, suggesting market normalization and stabilization.

Due to the year of execution of the study (December/2024), only the 2023 period will be considered from this point forward, to ensure a more focused analysis on recent trends and market conditions.

## Monthly analysis (2023)

| Month | Minimum Cost | Average Cost | Maximum Cost |
|:-:|:-:|:-:|:-:|
| 1 | 17.92 | 101.23 | 173.37 |
| 2 | 70.74 | 111.23 | 155.30 |
| 3 | 28.32 | 94.91 | 150.51 |
| 4 | 22.73 | 65.80 | 124.57 |
| 5 | 28.56 | 68.50 | 94.41 |

xxx

## Comparison of consumption

<p align="center"><img src="https://github.com/lucas-dpontes/Cost-Optimization-Analysis-for-Eesti-Energia/blob/main/heatmap-hour-day.png"></p><br>

It is observed that there is a predominance of consumption during the periods from 6-9 AM and 4-9 PM.

<br><br><h1 align="center">Conclusions & Insights</h1>

Suggestions to reduce production costs:
1. By analyzing the behavior of energy costs throughout the day, we observe that the average cost of energy is significantly cheaper between 10 PM and 5 AM, being almost three times cheaper than producing energy during commercial hours.
2. To take advantage of this cost difference, it is essential to expand the use of energy storage solutions, such as lithium-ion batteries, thermal energy storage systems, and gravitational potential energy. These solutions allow energy to be stored during periods of lower cost and used during peak hours, optimizing consumption and reducing operational costs.
3. Additionally, a change in the billing model can be beneficial. Offering lower rates during off-peak hours would encourage consumers to shift part of their consumption to these periods, promoting a more homogeneous distribution of energy consumption throughout the day. This would not only reduce the pressure on generation and distribution infrastructure during peak hours but also result in greater energy efficiency and lower costs for consumers.
