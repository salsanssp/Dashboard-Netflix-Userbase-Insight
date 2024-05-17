# Dashboard-Netflix-Userbase-Insight

![image](https://github.com/Vanz92x/Netflix-Userbase-Insight/assets/165736197/02d77413-ca5d-4eb4-bd6f-b33966bcee28)

## Data Visualization with Looker Studio
<div align="center"><img src="https://github.com/Vanz92x/Netflix-Userbase-Insight/assets/165736197/9c5a2fc9-a9c4-4e91-83c1-b71b882b4cec" /></div>

Looker Studio is a data analytics and visualization platform that allows users to create interactive reports and dashboards from various data sources. By using Looker Studio, users can connect, process, and visualize data to gain deeper insights and support better decision-making. This platform supports various integrations with popular data sources like Google BigQuery, Google Sheets, MySQL, and many more, making it easy for users to access and analyze data from multiple sources in one place. In this case, we are using Looker Studio to visualize this dataset.

## Why we are use Looker Studio?
* **Easy to use**

  Because it is website based, the features are also quite complete even though there are free features
* **Convenient Templates**

  There is a template feature that can be used, which can be used when you need quick visualization
* **Versatile and Customizable**

  Even though there are templates provided, users can also create their own visualizations.
* **Collaborate in real-time**

  By sharing Looker Studio files with other editors, you can work together simultaneously as a team.

## Business Understanding

**Background:**

The provided dataset represents a sample of Netflix's user base, detailing key attributes related to subscription types, user demographics, and usage patterns. This dataset is crucial for understanding Netflix's revenue streams, user engagement, and market penetration across different countries. By analyzing this data, Netflix can gain valuable insights into user behavior, preferences, and trends.

**Business Question:**

1. How many users are there by gender for each subscription type?
2. What is the percentage of users for each type of device?
3. What is the trend in monthly revenue?
4. What is the total annual revenue?
5. Which countries are in the top 10 by revenue?

## Data Understanding

Data of Netflix Userbase Insight from 09 May 2021 to 01 Desember 2023

Source data: https://www.kaggle.com/datasets/arnavsmayan/netflix-userbase-dataset/data 

The dataset has 13 columns and 9648 rows.

Data Dictionary:

* User ID: Unique identifier for each user netflix.

* Subscription Type: Type of subscription plan the user is enrolled in (e.g., Basic, Standard, Premium).

* Monthly Revenue: Revenue generated by users who subscribe monthly.

* Join Date: Date when the user joined the netflix.

* Last Payment Date: Date of the user's most recent subscription payment.

* Country: Country where the user is located.

* Age: Age of the user.

* Gender: Gender of the user.

* Device: Primary device used by the user to access the service (e.g., Mobile, Tablet, Smart TV, Laptop).

* Plan Duration: Total duration of the current subscription plan.

## Data Preparation

Code Used:
* Python Version: 3.11.7

* Packages: Pandas.

## Data Cleansing

<div align="center"><img src="https://github.com/Vanz92x/Netflix-Userbase-Insight/assets/165736197/5f55a673-c56b-438a-86a9-6ee23f4448b1" /></div>

The table above shows that there are no missing values, but the Join Date and Last Payment Date columns have incorrect data types. Therefore, we need to change their data types to datetime to ensure accuracy and ease of data processing. This will allow us to calculate time intervals more accurately and sort the data by date.

## Data Visualization and Story Telling

### How many users are there by gender for each subscription type?

<div align="center"><img src="https://github.com/Vanz92x/Netflix-Userbase-Insight/assets/165736197/a0deabb9-a7cf-4dee-bded-ad8c63e5cad9" /></div>

Based on the above bar chart, we can see that the **Basic subscription type dominates the number of users**. This may indicate that **the majority of Netflix users choose the most affordable subscription package**. Additionally, the number of subscription usage does not significantly differ between males and females, indicating that subscription **preferences are not gender-dependent**. This could be an indication that the content offered by Netflix has broad appeal, not limited to a specific gender.


### What is the percentage of users for each type of device?

<div align="center"><img src="https://github.com/Vanz92x/Netflix-Userbase-Insight/assets/165736197/63616204-89c5-45b7-b876-41541902224c" /></div>

From the above diagram, it can be seen that there are four types of devices used by users with percentage values that are not much different. On the other hand, **the device with the most percentage used by users is a laptop** as much as 25.4% while **the least used device is Smart TV** as much as 24.4%.

### How many users are there by gender for each subscription type?

<div align="center"><img src="https://github.com/Vanz92x/Netflix-Userbase-Insight/assets/165736197/41889093-e3c5-4523-9814-bcc0ddbf8440" /></div>


Based on the chart above, we can see that **the highest income is in October**, amounting to $6,604. **Meanwhile, February is the month with the least income generated by Netflix**, only $160. The significant difference between months is also caused by the variance in the amount of data, with data for 2021 starting only from September to December, while data for 2023 only displays January to June.

### What is the total annual revenue?

<div align="center"><img src="https://github.com/Vanz92x/Netflix-Userbase-Insight/assets/165736197/19f47b17-07f5-42e6-b3e7-e2bbe28be14f" /></div>


Based on the graph above, it can be seen that **2022 is the year with the highest revenue**, reaching 97.97%. **This increase is very significant and sharp compared to 2021 and 2023**. Since 2021 only has data from September to December, while 2023 only has data from January to June, both years show lower revenue.

### Which countries are in the top 10 by revenue?

<div align="center"><img src="https://github.com/Vanz92x/Netflix-Userbase-Insight/assets/165736197/81d0bff5-0a0f-450f-87e7-491c56757c7f" /></div>


Based on the chart above, we can see that the **United States is the country with the most netflix revenue** of $5,564 and **Mexico is the country with the least revenue** of $2,237.


## Summary

* The number of subscription types Basic has the highest value due to its more affordable price. In addition, subscription preferences do not depend on gender.
* The device with the most percentage used by users is a laptop as much as 25.4% besides that, the percentage difference between the devices used is very thin.
* 2022 is the year with the highest revenue, reaching 97.97%.
* United States is the country with the most netflix revenue of $5,564 and Mexico is the country with the least revenue of $2,237.
* The highest income is in October, amounting to $6,604. Meanwhile, February is the month with the least income generated by Netflix, only $160.
* The significant difference between months is also caused by the variance in the amount of data, with data for 2021 starting only from September to December, while data for 2023 only displays January to June.

