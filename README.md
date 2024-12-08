# PhoneNow-KPI-Dashboard

## Introduction
This is a **Power BI project** on call center performance analysis for an imaginary telecom organization called **PhoneNow**. The project aims to evaluate the efficiency and effectiveness of the call center operations by analyzing key metrics such as **overall customer satisfaction**, **calls answered vs. abandoned**, **average speed of answer**, and individual **agent performance**.
The goal is to identify trends, address inefficiencies, and provide actionable insights that can enhance customer service quality, optimize resource allocation, and improve overall call resolution rates. This analysis also includes recommendations to better manage peak hours, reward top-performing agents, and address common customer issues more efficiently.

## Problem Statement
PhoneNow is facing challenges in optimizing its call center operations to meet growing customer demands and ensure high satisfaction levels. The company needs to identify trends in call volumes, assess agent performance, and understand key factors affecting customer satisfaction and call resolution rates. The primary objective of this analysis is to provide actionable insights that enhance service quality, improve resource allocation during peak hours, and support the development of strategies to optimize overall call center performance.

## Data Exploration

| **Column**             | **Description**                                                                                       |
|-------------------------|-------------------------------------------------------------------------------------------------------|
| **Call Id**            | Unique identifier for each call.                                                                     |
| **Agent**              | Name of the call center agent handling the call.                                                     |
| **Date**               | Date the call was made.                                                                              |
| **Time**               | Exact time the call was initiated.                                                                   |
| **Topic**              | Main issue discussed during the call.                                                                |
| **Answered (Y/N)**     | Indicates whether the call was answered (Y) or not (N).                                              |
| **Resolved (Y/N)**     | Indicates whether the issue was resolved during the call (Y) or not (N).                              |
| **Speed of Answer (seconds)** | Time taken (in seconds) for the agent to answer the call after it was initiated.                   |
| **Avg Talk Duration**  | Average duration of the call in hours, minutes, and seconds.                                         |
| **Satisfaction Rating** | Customer's rating of the call experience on a scale of 1-5.                                          |
