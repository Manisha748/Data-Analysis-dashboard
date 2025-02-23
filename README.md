# Data-Analysis-dashboard

# Project Description

A Power BI dashboard analyzing key factors affecting affordable healthcare, including hospital costs, insurance coverage, survival rates, financial assistance impact, and patient satisfaction scores.


# Affordable Healthcare dashboard

### Dashboard Link :https://github.com/Manisha748/Data-Analysis-dashboard/blob/main/afford_heathcare.pbix
## Problem Statement

Healthcare affordability remains a significant challenge, particularly for low-income individuals who require critical financial support. High medical costs, limited insurance coverage, and dissatisfaction with treatment methods contribute to increased financial strain and poor health outcomes.

By leveraging data-driven insights, this analysis seeks to identify the key reasons behind gaps in insurance coverage and maximize insurance support for vulnerable groups while maintaining balance across other categories. The goal is to enhance healthcare accessibility and affordability by addressing financial, institutional, and treatment-related barriers.


# Questions (KPI's)
1️) Most affordable or least expensive hospital type.

2️) Age group with illness.

3️) Maximum insurance coverage for teenagers with disease, providing affordable healthcare.

4️) Maximum insurance coverage for the low-income level category.

5️) Find if there is a relation between survival outcome and income level to identify deaths due to unaffordability.

6️) Find the survival rate if the strategy of providing maximum financial assistance decreases death rates.

7️) Identify the most critical disease (most expensive and least probability of success in cure).

8️)Identifying the cause for low satisfaction rates, such as unsuitable treatment or the need to switch to other treatment methods.


### Steps followed 

- Step 1 : The dataset is in a CSV file and is imported into Power BI Desktop.
- Step 2 : Duplicates and null values were removed from all columns to ensure data integrity.
- Step 3 : After applying necessary transformations, click "Close & Apply" in Power Query Editor to load the cleaned data into Power BI.

- Step 4 :A star schema was designed with fact_treatment as the central fact table and the following dimension tables:
  1)dim_hospital – Contains hospital-related details.
  2) dim_insurance – Stores information on insurance coverage.
  3)dim_patient – Holds patient demographics and health conditions.

- Step 5 : A new visual was added for representing different health conditions using age groups in the Visualizations pane.
- Step 6 : Visual filters (Slicers) were added for the fields:
  "Adults"
  "Middleage"
  "Seniorcitizen"
  "Teenage".
- Step 7 :  Two multi-row card visuals were added:
  Q1, Median, and Q3 for each Hospital Type
  Survival Rate Before vs. Survival Rate After Assistance

- Step 8 : A card visual was created to display the correlation between Income Level and Survival Outcome.
  The result showed a very weak positive correlation, indicating almost no linear relationship between Income Level and Survival Outcome in the dataset.
  
 
  
In our dataset, some parameters were assigned values 0 and 1, representing that those parameters are not applicable for measures like SUM or AVERAGE.

The records for each hospital type were unbalanced, meaning some hospital types had significantly more data points than others.


# Snapshot of Dashboard (Power BI Service)

![dashboard_snapo]https://github.com/Manisha748/Data-Analysis-dashboard/blob/main/affordhealth.png




#  Project Conclusion
1)Government hospitals are the cheapest across all quartiles.

Nonprofit hospitals have the highest costs, especially in the upper range.

Private hospitals are in between, slightly more affordable than nonprofits but more expensive than government hospitals.

• For affordability, government hospitals are the best choice.

2)Middle Age follows, also with many Chronic Diseases and Acute Illnesses.

Adults have fewer illnesses compared to Seniors and Middle Age groups.

Teenagers have the least illnesses overall.

• Senior Citizens have the highest total illnesses (Chronic Diseases are dominant).
Emergency (Red Bubble) is the most critical condition.

3)Emergency has the lowest survival rate and the largest bubble size (likely representing death rate).

Acute Illness (Light Blue) and Chronic Disease (Dark Blue) have higher survival rates and smaller bubbles, meaning they are less critical.

Emergency is the most critical condition because:

1. Lowest survival rate

2. Highest death rate (largest bubble)

3. Comparable or slightly higher normalized cost

4)r=1 Strong positive correlation (as one variable increases, the other also increases).

r=-1 Strong negative correlation (as one variable increases, the other decreases).

r≈0  No correlation (no linear relationship between the variables).

r = 0.01 → Very weak positive correlation, meaning there is almost no linear relationship between Income Level and Survival Outcome in the data.

5)The decrease in survival rate after financial assistance is not necessarily because financial aid is ineffective.

Key Reasons for the Drop:

Patients Who Previously Received Assistance No Longer Qualify

Some patients who were previously assisted and survived may no longer receive aid under the new criteria.


