# Performing a Cluster Analysis to Determine how Baltimore City Agencies are Grouped FY2019
## Background
The City of Baltimore offers the opportunity to work in various roles. While all departments have the same end goal to serve the city, not all positions are paid equally. It is interesting to consider whether we expect similar agencies to have similar average compensation, and whether number of years worked may be related to pay. We’ll take a look at Baltimore City salary data to determine how different agencies are grouped together.

## Business Question
***Can we determine how different Baltimore City agencies are grouped together based on annual salary, gross salary, and number of years worked for the fiscal year 2019?***

## Data Sources
We looked at Baltimore City Employees Salaries data from [Open Baltimore](https://data.baltimorecity.gov/City-Government/Baltimore-City-Employees-Salaries/w28m-utix). We took the [raw data](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/Baltimore_City_Employees_Salaries_RawData.xlsx) and [filtered it](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/Balti_Employees_Salary_Manipulated.xlsx) to look at annual salary and gross pay in addition to the number of hours worked. In order to perform [our cluster analysis,](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/Balti_Employees_Cluster_Analysis.xlsx) we grouped roles together by agency to [find the average](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/Balti_Employees_DataVisuals.xlsx) of each variable, resulting in 57 departments.

## Data Analysis
1. Annual Salary is the average annual salary of each agency
2. Gross Pay is the average amount actually paid in compensation
3. Years Worked is the average number of years worked 

**How is our data clustered?**
![insert](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/clustering%20results.png)
We chose to create four anchors in order to find our separate cluster categories. As a result of our analysis, we can see that each agency was assigned to one of the four cluster nodes based on their minimum z-score distance.

The positive and negative z-scores tells us how each cluster fares in terms of being higher or lower than average for each variable. The Health Department cluster 1 has lower than average salary, gross pay, and number of years worked. The Comptroller's Office cluster 2 has higher than average salary and gross pay, and much greater than average number of years worked. The Human Resources cluster 3 has higher than average salary and gross pay, but lower than average number of years worked. Finally, the Recreation cluster 4 has much lower than average salary, gross pay, and number of years worked.

**What do these clusters mean?**
![insert2](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/cluster%20table.png)

This table shows us the groupings of our cluster analysis. We can see that the clusters seemed to be grouped by similar job responsibilities. Cluster 1 is made up of departments that are focused on community services, cluster 2 is administration and first responders, cluster 3 is primarily civil servants, and cluster 4 appears to be generally lower-skilled roles. 

**What does average annual salary, gross pay, and years worked look like for all departments?**

![insert3](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/average%20annual.png)

![insert4](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/average%20gross%20pay.png)

![insert5](https://github.com/katiesunsg/baltimore-employees-salary-fy2019/blob/main/average%20years%20worked.png)

The bar graphs above give a visual representation of average salary, pay, and years worked. We can see that most departments make an average of ~$50k with ~10 years worked. While some departments such as Council Services have higher than average salary and higher than average number of years worked, on the other hand, the Transportation - Highways department has the third highest number of years worked but lower than average pay. In addition, cluster 2 and 3 are being respectively above and below the average number of years worked, yet both have higher than average pay.

## Summary
Our findings mean that similar types of agencies is a greater indication of how departments are grouped together in a cluster analysis, rather than number of years worked. This data might be important for organizations seeking transparency on how Baltimore City agencies are paid, such as unions advocating for more equitable pay or concerned citizens wanting to see where their taxpayer money goes. Additional data that might be useful for further analysis would be averaging based on role to determine entry-level vs. executive-level pay discrepancies, as well as breaking down number of years worked further to determine whether it accounts for upwards mobility within or between departments.
