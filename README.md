# PhoneNow-KPI-Dashboard

## Introduction
This is a **Power BI project** on call center performance analysis for an imaginary telecom organization called **PhoneNow**. The project aims to evaluate the efficiency and effectiveness of the call center operations by analyzing key metrics such as **overall customer satisfaction**, **calls answered vs. abandoned**, **average speed of answer**, and individual **agent performance**.
The goal is to identify trends, address inefficiencies, and provide actionable insights that can enhance customer service quality, optimize resource allocation, and improve overall call resolution rates. This analysis also includes recommendations to better manage peak hours, reward top-performing agents, and address common customer issues more efficiently.

## Problem Statement
PhoneNow is facing challenges in optimizing its call center operations to meet growing customer demands and maintain high satisfaction levels. Key issues include:

- Identifying trends in call volumes and agent performance.
- Understanding factors affecting customer satisfaction and resolution rates.
- Reducing unanswered and abandoned calls during peak hours.

The primary objective is to provide actionable insights that enhance service quality, optimize resource allocation during peak hours, and support the development of strategies to improve overall call center performance.

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

## METHODOLOGY
### Data Preparation and Transformation
1. ETL Process: Data was extracted, transformed, and loaded into Power BI.
2. Data Cleaning: Replaced missing values, standardized column formats, and added conditional columns.
3. Calculated Measures: Developed custom DAX measures for KPIs.
4. Filters and Slicers: Enabled filtering by Agent, Topic, and Time Period for dynamic analysis.

### Data Modelling
To enable robust time intelligence and facilitate a detailed analysis of the performance of the call center, the data preparation process was conducted with precision and attention to detail. Key activities included:  

- **Calendar Table Development**: A custom calendar table was created to support advanced time-based analytics.  
- **Dataset Integration**: The calendar table was seamlessly integrated with the marketing campaign datasets for cohesive analysis.  
- **Relationship Mapping**: Relationships were established between the calendar table and other data tables through shared date columns, ensuring consistent linkage.  
- **Data Model Validation**: A thorough review of the data model was conducted to confirm data integrity and ensure the accuracy of relationships.  

This structured approach laid the groundwork for meaningful insights through accurate and comprehensive visualizations.

## Data Model

![Model](images/CallcenterModelling.JPG)

## Raw Data Preview

![Preview](images/Data_Preview.JPG)

## Report Structure
The dashboard consists of two pages for focused analysis:

1. Call Center Performance Overview: Provides high-level metrics, including total calls, abandonment rates, busiest hours, and topic distribution.

2. Agent Performance and Topic Analysis: Focuses on individual agent performance, satisfaction ratings, handle time, and a detailed breakdown of topics handled by the call center.

## Key Insights
The analysis provides detailed insights into PhoneNow's call center operations over three months (January–March 2021), focusing on critical metrics such as call handling efficiency, agent performance, customer experience, and topic trends.

### Call Handling Efficiency
- Total Calls: 5000 calls were logged over the three-month period.
- Answered Calls: 4054 calls (81.08%) were successfully answered by agents. This highlights a generally efficient response rate but leaves room for improvement.
- Resolved Calls: Of the answered calls, 3646 (72.92%) were resolved during the initial interaction, indicating effective problem-solving for most cases.
- Abandoned Calls: 946 calls (18.92%) were abandoned before an agent could respond, a potential area of concern, especially during peak hours.

### Agent Performance
- Top Performer: Jim handled the highest number of calls (536), resolving 485, showcasing consistent performance.
- Highest Customer Satisfaction: Martha achieved the highest average satisfaction rating of 3.47 out of 5, reflecting excellent customer engagement and problem resolution skills.
- Average Handle Time: Across all agents, the average time to handle a call ranged between 223 and 231 seconds, demonstrating relatively consistent efficiency among team members.
- Underperforming Metrics: Some agents displayed lower satisfaction ratings and resolution rates, suggesting the need for targeted coaching.

### Customer Experience
- Average Satisfaction Rating: Customers rated their experiences at an average of 3.40 out of 5, highlighting room for improvement in service quality.
- Average Speed of Answer: Calls were answered within 67.52 seconds on average. However, during peak periods, delays likely contributed to higher abandonment rates.
- Key Performance Hours: The busiest times were identified as 13:00–14:00, followed by 11:00–12:00 and 17:00–18:00. These periods saw the highest call volumes and longest response times.

### Topic Analysis
- Common Issues: The majority of calls were related to "Streaming" (749 calls), "Technical Support" (736 calls), and "Payment-related" issues (729 calls). This indicates recurring areas of concern that demand focused attention.
- Resolution Challenges: Calls related to technical support showed slightly lower resolution rates, suggesting the need for specialized agent training in this domain.

### Call Abandonment Trends
- Critical Hours: Unanswered calls peaked between 12:00–13:00 and 09:00–10:00, coinciding with high call volumes and insufficient staffing.
- Impact on Satisfaction: High abandonment rates during these hours could significantly impact customer satisfaction and loyalty if left unaddressed.
