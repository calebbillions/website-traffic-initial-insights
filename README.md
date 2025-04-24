# website-traffic-initial-insights
This report presents an exploratory analysis on Website traffic gotten from Kaggle, focusing on uncovering key insights and observations.


## **Table of Contents**
  - [Introduction](#introduction)

  - [Dataset Overview](#dataset-overview)

  - [Tools and Methodology](#tools-and-methodology)

  - [Key Insights](#key-insights)

  - [Conclusion](#conclusion)


## Introduction
This analysis report reviews marketing data sourced from Kaggle, an online repository widely used by data professionals. The primary objectives of the initial exploratory data analysis (EDA) were to:
1. Characterize the Dataset
  -  Examine the overall structure, data types, and feature composition
  -  Assess completeness and basic statistical properties of each variable

2. Uncover Patterns and Insights
  -  Identify correlations, trends, and anomalies among marketing metrics
  -  Highlight key drivers of performance and potential areas for further investigation

## Dataset Overview
The Dataset is on Website Traffic and contains 2000 rows and 7 columns based on website user behaviour and engagement metrics. Below is a breakdown of the different columns contained in the data and a brief description:
##   Brief description of the dataset
![Image](https://github.com/user-attachments/assets/d9fa7421-d5de-4130-8fdb-221f233a50ec)
1. **Page Views**: The number of pages viewed during a session.
(this indicates the engagement level of the visitors by showing how many pages they visit during their session)

2. **Session Duration**: The total duration of the session in minutes.
(measures the length of time a visitor stays on the website, which can indicate the quality of the content)

3. **Bounce Rate**: The percentage of visitors who navigate away from the site after viewing only one page.
(A critical metric for understanding user behavior. A high bounce rate may indicate that visitors are not finding what they are looking for)

4. **Traffic Source**: The origin of the traffic (e.g., Organic, Social, Paid).
(Understanding where your traffic comes from can help in optimizing marketing strategies)

5. **Time on Page**: The amount of time spent on the specific page in minutes.
(This helps in analyzing which pages are retaining visitors’ attention the most)

6. **Previous Visits**: The number of previous visits by the same visitor.
(This can be used to analyze the loyalty of visitors and the effectiveness of retention strategies)

7. **Conversion Rate**: The percentage of visitors who completed a desired action (e.g., making a purchase).
(The ultimate metric for measuring the effectiveness of the website in achieving its goals)


## Tools and Methodology
-  ## Tools:
    -  **Python:** I utilized it for data loading, processing, analysis, and visualization.

    -  **Jupyter Notebook**: It served as the development environment, with the .ipynb file attached to this repository.

    -  **Libraries**: pandas for data manipulation, numpy for numerical operations, matplotlib and seaborn for visualization.

-  ## Methodology:
    -  **Data Loading**: I imported the marketing dataset into Python using pandas.

    -  **Data Validation**: I checked data types and ensured consistency across features.

    -  **Exploratory Analysis**: I computed summary statistics to understand central tendencies and dispersions.

    -  **Visualization**: I generated box plots to detect outliers and examine distributions, alongside other chart types to reveal patterns.  


## Key Insights
### 1. Page views
  -  ![Image](https://github.com/user-attachments/assets/685d7743-9cc6-42db-a45b-a0dc83cf9bef)
  -  It is observed that users spend an average of 4.95 views, approximately 5 page views per session. It can also be observed that 50% of the visitors view between 3 to 6 pages per session, suggesting these are users that explore beyond the landing page and find engaging content there. The maximum number of page views in the box plot is 10

### 2. Session Duration
  -  ![Image](https://github.com/user-attachments/assets/101cbced-0ff1-4451-be61-70df7620f575)
  -  The average session duration on the website is approximately 3 minutes. 50% of the visitors last between 0.8 minutes (48 seconds) and 4.2 minutes on the website, below 5 minutes.

### 3. Bounce Rate
  -  ![Image](https://github.com/user-attachments/assets/5cd71098-f89e-48d9-9b8d-1467be377231)
  -  An average bounce rate of 28.5% across pages shows that a significant portion of visitors engage with multiple pages, likely finding the content relevant. 50% of users have bounce rate values ranging between 16.2% and 38.9% showing that most pages retain visitors.

### 4. Time on Page
  -  ![Image](https://github.com/user-attachments/assets/d7d7302f-2990-4b12-bdc4-a8cfd97b9d55)
  -  The average time spent on a page is approximately 4 minutes, indicating a reasonable level of engagement. 50% of users spend between 2 and 5 minutes on a page, suggesting that most visitors stay long enough to interact with the content.

### 4. Previous Visits
  -  ![Image](https://github.com/user-attachments/assets/343f61e8-821a-42ac-b945-25813bab7397)
  -  On average, users have approximately 2 previous visits, indicating a moderate level of returning visitors. 50% of visitors have between 1 and 3 previous visits, suggesting that many visitors are new.
25% of users have more than 3 previous visits, suggesting they are loyal visitors. There are a few outliers, with the maximum recorded previous visits reaching 9.

### 5. Conversion Rate
  -  ![Image](https://github.com/user-attachments/assets/18188779-a636-4167-ba40-67bfe6a8c40b)
  -  The average conversion rate is 98.2%, meaning that nearly all visitors complete a desired action. While this could indicate an exceptionally well-optimized website, it is also important to investigate factors influencing this and to check what actions are categorised as “conversions”.

### 6. Traffic Source
  -  ![Image](https://github.com/user-attachments/assets/6a93e3f1-62b1-400a-aec5-c5c12610e400)
  -  Organic traffic is the dominant source, with 786 visits. Paid traffic with 428 visits, shows that investment in paid advertising is driving a significant portion of users to the site. Referral traffic for 301 visits, Social traffic, with 269 visits, plays a smaller role but still brings in visitors. Direct traffic, at 216 visits, is the lowest among the sources and it represents users who enter the website URL directly.

### Multivariate Analysis
  -  I used a heatmap to visualize pairwise relationships and identify significant positive or negative associations.
  -  ![Image](https://github.com/user-attachments/assets/3791d667-0329-49ee-b4f5-ec8e65a6d335)
  -  The heatmap indicates that most feature correlations are weak. The strongest positive relationships are between Session Duration and Time on Page (**0.23**) and between Session Duration and Conversion Rate (**0.18**). Overall, none of the features demonstrate strong interdependence.

## Conclusion
-  Initial examination of the website traffic data reveals numerous outliers across the numerical columns, each of which warrants closer inspection. In particular, the unusually high conversion rates should be scrutinized to determine which actions were classified as “conversions.” Additionally, further analysis will explore the relationships among all features to understand how they interact and influence one another.




