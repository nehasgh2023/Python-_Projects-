**Case Study**
This is a U-food Marketing Data Analysis project. where we are solving a case study of UFood which is a leading food delivery app in Brazil having its presence over thousand cities. 
In this case we are presented with a sample dataset, that mocks metainformation on the custoemr and UFood campaign with that customer.
We are given a challenege to understand the data, find business opportunities and insights to propose any data driven action to optimize the campaign results and generate value to the company. 

They key objectives of this project are:
1) Explore the data, provide insights, define cause and effect.
2) Propose and describe a customer segmentation based on customers behaviors.
3) Visualize data and provide written reasoning behind discoveries.

**Solution
Exploratory Data Analysis in pandas.**
i imported the data in dataframe 'food' in pandas.
Checked for the duplicates.
**Dropped the found duplicates.**
 arranging and combining the columns. 
1. Combined the kidshome and teenhome column.
2. Gave numbers to the marital status and putting all the marital status data in 1 column and created another column called Marital_Status_str where we mapped the number with the statuses.
3.Did the same thing with educational level.
4. Did the same thing with Accepted Campaigns

**Correlation Analysis**
for correlation analysis we need to make sure that all the columns have numerical data.
i applied 'pearson'correlation on the dataframe. '0' correlation means no relationship. 
i tried to show the correlation data which are >0.3 in a heatmap using seaborn library. The number 0.3 was assumed to be a threshols to check correlation. 
i also checked the correlation of people who "Accepted Campaigns" with other columns in the dataset.

**Customer Segmentation**
-> created a new column with Age_Group data and also calculated the percentage of those age groups.

-> Visualized the age group with the accepted campaigns in barplot using matplotlib library in python.
   i found out that the age group accepting most campaigns are between 31-70. especially 41-50 haev highest accepted data.

-> Now finding the relation between age group and money spent : no concrete conclusion was made from the plot.
-> finding where do people spend more i.e store, catalog, web:
    created a new dataframe to find out the number of web,store and catalog purchas with accepted campaigns 
    PLotting the data in a bargraph shows that people who are accepting campaigns have high instore purchses.
    The catalog purchases are higher than the web purchases which means that people who are accepting the catalog purchase. I could mean that people who are accepting campaigns are making more catalog purchases.
    i used joint plot to see the relationship beween the accepted campaigns and purchases.
-> Now i tried to find out kids with the accepted campaigns relationshio. Plotting in reg plot the total children vs accepted campaigns is seen that there is a negative correlation. 
  it means that people who ahve more children are less likely to accept more campaigns.
  -> Education status with the Accepted Campaigns and Mnt total showed no significant difference.
  -> Marital Status : the count of married people in the dataset was higher than the other.the people with marrital status 'married' accepted more campaigns and spent more money.
  
   OVERALL FINDINGS
1.Age = 30-70 were spending more money, but less likely to accept campaigns.Higher volume here though.
2.Catalog was more likely to accept campaigns but in person spend more. Recommend a split between all.
40% catalog, 30% store and 30% web
3.Focus on people with no kids(or less kids)
4.Education: No impact-don't target any group
5. Marital Status: Doesn't play a big part. Married, Single, Together, spend more money
Money Making
middle aged people, high earners, with no kids. Target on different platforms with split above
New Users to Spend Money
Focus on 23-30, 70 and up- who statistically accepted campaigns at higher rate.

In this project i have used pandas, matplorlib, seaborn as python libraries to attamept this EDA on Ufood Maketing Data. 



 
