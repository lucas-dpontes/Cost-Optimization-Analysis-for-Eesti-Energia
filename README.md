# Cost-Optimization-Analysis-for-Eesti-Energia

Data analysis project developed as part of the Eesti Energia challenge, promoted by the **[Data Vinking](https://www.dataviking.com.br/)** data community. 

This document summarizes the trajectory of the data analysis project, highlighting the main points and visualizations.

The complete study is available clicking here, or by accessing the file Project.ipynb located in this repository.

Project developed by Lucas Pontes *[profile](https://www.linkedin.com/in/lucasdpontes/)*

<br><br><h1 align="center">Introduction</h1>

Eesti Energia AS is an energy company located in Estonia. It is the largest oil shale energy company in the world.

In 2014, it operated in Estonia, Latvia, Lithuania, Finland, Jordan, and Utah (United States).

The group has three main areas of operation:
- electricity generation
- oil shale production
- electricity sales and distribution

Business Pain: high production cost
Root Cause: high energy cost
Main Goal: study the energy cost data and suggest an action plan to reduce the cost

<br><br><h1 align="center">Analysis</h1>

## Annual average price

<div align="center">

| Year | Average price [€] |
|:-:|:-:|
| 2021 | 137.2 |
| 2022 | 192.8 |
| 2023 | 86.2 |

</div>

A peak period was observed in 2022, followed by a sharp decline in 2023. It is advisable to analyze these variations more deeply.

## Moving average of prices

------------------------------------------IMAGEM

Based on the graph above, it can be observed that there is a significant variation in prices, with sharp peaks in 2022, followed by a gradual decline and stabilization in 2023.

The daily data (gray line) shows high fluctuations, while the weekly (blue line) and monthly (green line) averages smooth out the variations, highlighting long-term trends.

The observed peaks, particularly in 2022, may be linked to energy crises or external factors affecting the market, such as increased demand or supply restrictions.

From 2023 onwards, prices exhibit lower volatility and reduced levels, suggesting market normalization and stabilization.

Due to the year of execution of the study (December/2024), only the 2023 period will be considered from this point forward, to ensure a more focused analysis on recent trends and market conditions.

## Monthly analysis of 2023:

Then, turnover cycles were identified, according the chart below, to highlight specific periods in which there were spikes in employee departures from the company.

**according to available data, turnover cycles were analyzed based on the hiring date.*

<details>
  <summary>Code</summary>
  
```
xxx
```
</details>

Based on the hiring history, this value was increased in the 4th quarter of 2023.

In the second quarter of 2024, specifically on March 15, there were 144 layoffs, indicating a **possible mass layoff** scenario.

## Risk profile

In addition, the risk profile of employees was investigated, comparing those who left the company with those who stayed to understand whether higher satisfaction or performance were directly related to these departures.

<div align="center">

| | Former employee | Current employee |
|:-:|:-:|:-:|
| **Avg performance (0-5)** | 2.94 | 3.32 |
| **Avg satisfaction (0-5)** | 2.96 | 2.89 |

</div>

<br><details>
  <summary>Code</summary>
  
```
# Dataframe creation
xxx
```
</details>

<p align="center"><img src="https://github.com/lucas-dpontes/People-Analytics-Challenge/blob/main/avg_satisfaction_performance_work.PNG?raw=true" width=700></p><br>

<details>
  <summary>Code</summary>

  ```
  # Dataframe creation
xxx
```
</details>

<p align="center"><img src="https://github.com/lucas-dpontes/People-Analytics-Challenge/blob/main/avg_satisfaction.png?raw=true" width=700></p><br>

<details>
  <summary>Code</summary>

  ```
# Dataframe creation
xxx
```
</details>

<p align="center"><img src="https://github.com/lucas-dpontes/People-Analytics-Challenge/blob/main/avg_performance.png?raw=true" width=700></p><br>


<details>
  <summary>Code</summary>

  ```
# Dataframe creation
xxx
```
</details>

<p align="center"><img src="https://github.com/lucas-dpontes/People-Analytics-Challenge/blob/main/salary-position.png?raw=true" width=700></p><br>

According to the boxplot views above:
- There is no significant difference between the salaries of former and current employees, regardless of position;
- Also regardless of position, people with higher performance are formers;
- Senior people with lower satisfaction tend to leave their jobs, probably because they found better opportunities.

## Correlations

Statistical analyzes were also carried out to identify correlations between the variables in the database, seeking to better understand the factors underlying high turnover.

<details>
  <summary>Code</summary>

```
xxx
```
</details>

<p align="center"><img src="https://github.com/lucas-dpontes/People-Analytics-Challenge/blob/main/heatmap-corr.png?raw=true"></p>

## Employees with 2+ years at the company

Finally, employees with up to 2 years at the company were compared with those with 2+ years, seeking to identify possible discrepancies that could provide additional insights about retention.

<details>
  <summary>Code</summary>
  
```
# Flag for employees over 2 years old
xxx
```
</details>

<p align="center"><img src="https://github.com/lucas-dpontes/People-Analytics-Challenge/blob/main/avg_salary_position.png?raw=true" width=500 height=420></p><br>

<details>
  <summary>Code</summary>
  
```
# Dataframe creation
xxx
```
</details>

<p align="center"><img src="https://github.com/lucas-dpontes/People-Analytics-Challenge/blob/main/profile_months.png?raw=true" width=500></p><br>

<details>
  <summary>Code</summary>
  
```
xxx
```
</details>

<p align="center"><img src="https://github.com/lucas-dpontes/People-Analytics-Challenge/blob/main/histogram_profile_months.png?raw=true" width=500></p><br>

<details>
  <summary>Code</summary>
  
```
xxx
```
</details>

<div align="center">
  
| | Until 2 years | 2 years + |
|:-:|:-:|:-:|
| **Avg overtime hours** | 10.00 | 10.29 |
| **Avg performance (0-5)** | 3.05 | 2.99 |
| **Avg satisfaction (0-5)** | 2.93 | 2.96 |

</div>

<br><br><h1 align="center">Conclusions</h1>

After analyzing the profile of former and current employees, it was observed that all former employees left the company on the same day, indicating a collective action or a mass organizational decision. Furthermore, it was found that the average satisfaction of former employees was significantly lower than that of current ones, reducing a possible relationship between dissatisfaction and leaving the company.

Surprisingly, it was found that the performance of formers, on average, higher than that of currents. This may suggest that factors other than job performance are contributing to staff turnover, such as organizational culture issues, lack of growth opportunities, or misalignment of expectations.

It was identified that the proportion of employees with more than 2 years is significantly higher than the opposite.

These findings highlights the importance of a multidisciplinary approach to talent retention that takes into account not only individual performance, but also employee engagement, satisfaction and well-being. By addressing these aspects, organizations can create a more positive and motivating work environment, thus reducing employee turnover and promoting a effective retention.

For future steps, it is suggested to interview former and current employees.
