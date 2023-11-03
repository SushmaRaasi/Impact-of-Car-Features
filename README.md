# Impact-of-Car-Features

### Project Description
<p>The project aims to analyze a dataset of car features and prices to provide insights to a car manufacturer on optimizing pricing and product development decisions while meeting consumer demand.
</p>

### Business Problem
<p>The client wants to understand the relationship between car features, pricing, and market categories to maximize profitability.</p>

### DataSet
[Car Dataset](https://docs.google.com/spreadsheets/d/1uQz4v-BhwV0ChWCVO8qlJbOx3gw2QkWt4_4sowCqR_E/edit#gid=1723265621)

### Data Assumptions
<ul>
  <li>Completeness:</li>
  <p>I assume that the dataset is complete and doesn't have significant missing data. If there are missing values, I might assume that they are missing at random or have a specific pattern.</p>
  <li>Accuracy:</li>
  <p>I assume that the data is accurate and that errors or inaccuracies are minimal.
</p>
  <li>Consistency:</li>
  <p>I assume that the data is consistent over time or across sources. Changes in data collection methods or definitions can affect consistency.
</p>
  <li>Independence:</li>
  <p>You might assume that observations are independent of each other, especially in time series or experimental data.
</p>
  <li>Homoscedasticity:</li>
  <p>In regression analysis, you might assume that the variance of the errors is constant across all levels of the independent variables.
</p>
  <li>Model Linearity:</li>
  <p>In linear regression, you assume a linear relationship between the dependent and independent variables.
</p>
</ul>

### Approach
<p>For this project I used a mix of techniques. I relied on Microsoft Power BI to visualize data, analyze statistics and clean the data. I chose these methods because they allowed me to get an understanding of the dataset and make decisions on pricing and product development for a car manufacturer.
</p>
<p>Reasoning for using Analytical Methods
</p>
<ul>
  <li>Microsoft Power BI for Visualization:</li>
  <p>I went with Power BI because it's like an all-in-one solution. I could do everything from data cleanup to creating eye-catching charts without switching between different tools. It saved me time and helped me see the big picture.
</p>
  <li>Challenges and Limitations:</li>
  <p>Of course, no project is without its hurdles. I had to figure out what to do with missing data, make sure the data was accurate, and choose the best models for the job. Plus, the data had some limitations. Sometimes we didn't have all the pricing history we wanted, or we didn't know everything about consumer behavior. These challenges and limitations were like puzzle pieces that I had to work around to give the best recommendations I could.</p>
</ul>

### Tech-Stack Used
<p>To complete this project, I relied on a combination of tools and software to effectively manage and analyze the data. Here's a breakdown of the tech stack I used:
</p>
<p><i>Microsoft Power BI:</i> This was the star of the show when it came to data visualization and analysis. Power BI's user-friendly interface made it easy for me to explore the data, clean it up, and create insightful visualizations. It's like having a powerful magnifying glass to zoom in on the data's hidden patterns.
</p>
### Data Cleaning
<p>
  Data cleaning and preprocessing are essential steps in preparing a dataset for analysis.These steps help ensure that the data is accurate, consistent, and ready for meaningful analysis.
</p>
data cleaning image

### Insights

<ol>
  <li>The popularity of a car model vary across different market categories
</li>
  1.1
  1.2
  1.3
  <ul>
    <li>Based upon the above visuals Crossover category has a large number of models that is 1110 and some market Categories have lower number of models.</li>
  <li>Market Categories like Flex Fuel and Luxury having the number of models like 872 and 855 respectively.</li>
  </ul>
<li>The relationship between a car's engine power and its price</li>
  2
  <p>Based upon the trend line  Above visual there is a strong relationship between Engine HP and MSRP. If Engine HP increases then there is a tendency to increase in MSRP.
</p>

<li>Which car features are most important in determining a car's price
</li>
3
<p>Here I am doing Linear Regression Analysis. It is a statistical method used in data analysis to examine the relationship between one or more independent variables and a dependent variable. It is a valuable tool for understanding and quantifying the association between variables and making predictions or inferences.
</p>
3.1
<p>The Formula would be the same, just we need to change the Independent Variable.
Dependent Variable is MSRP. I used The DAX Formula to find the Coefficients.
</p>
<ul>
  <li>
    Engine HP_Coefficient: For every unit increase in Engine HP, MSRP increases by approximately 0.0012 units.
3.2
  </li>
  <li>City MPG_Coefficient: For every unit increase in City MPG, MSRP decreases by approximately 0.0000236 units.</li>
  <li>Engine Cylinders_Coefficient: For every unit increase in Engine Cylinders, MSRP increases by approximately 0.0000158 units.
</li>
  <li>Highway MPG_Coefficient: For every unit increase in Highway MPG, MSRP decreases by approximately 0.0000236 units.
</li>
  <li>Popularity_Coefficient: For every unit increase in Popularity, MSRP decreases by approximately 0.0012 units.</li>
  <li>In order to confirm I did t tests and got 0 for all p values.</li>
  3.3
  <li>Engine HP, City MPG, Engine Cylinders, Highway MPG, and Popularity all have statistically significant relationships with MSRP.
</li>
  <li>For Engine HP and Engine Cylinders, an increase in these variables is associated with an increase in MSRP.
</li>
  <li>For City MPG, Highway MPG, and Popularity, an increase in these variables is associated with a decrease in MSRP.</li>
  <li>These results suggest that these car features are important in determining the price of cars (MSRP), and the relationships are statistically significant.
</li>
</ul>

<li>How does the average price of a car vary across different manufacturers?
</li>
4
<li>What is the relationship between fuel efficiency and the number of cylinders in a car's engine?</li>
5
<ul>
  <li>72.94 + -65.3x: This part of the text indicates the equation of the trendline that's been fitted to your scatter plot. It's essentially a linear equation of the form y = mx + b, where:</li>
  <ul>
    <li>72.94 is the intercept (the value of y when x is 0).</li>
    <li>-65.3 is the slope (the coefficient that multiplies x). This represents the rate of change in the dependent variable (y) for a one-unit change in the independent variable (x). In this case, it suggests that for every unit increase in x, there is a decrease of approximately 65.3 units in y.</li>
  </ul>
  <li>|R2: 0.32|: The "R-squared" value measures the goodness of fit of our regression model. It tells you how well the trendline fits the data points. An R² value of 0.32 means that approximately 32% of the variability in the dependent variable (y) can be explained by the independent variable (x). In other words, the trendline explains some, but not all, of the variance in the data.</li>
  <li>corr: -0.57: This is the correlation coefficient (corr), and it quantifies the strength and direction of the linear relationship between the two variables. In this case, the correlation coefficient is approximately -0.57, which indicates a moderate negative correlation. A negative correlation suggests that as one variable (x) increases, the other variable (y) tends to decrease.</li>
  <li>n: 146: The "n" represents the sample size, which is the number of data points or observations used in your scatter plot and regression analysis. In this case, there are 146 data points.
</li>
</ul>
<p>So, to summarize, the equation 72.94 + -65.3x describes the linear relationship between the variables on your scatter plot. The R² value of 0.32 indicates how well this equation fits the data, and the correlation coefficient of -0.57 shows the direction and strength of the relationship. Finally, "n: 146" tells you the number of data points used in this analysis.
</p>
</ol>

### Snapshots of Dashboard

[Click here to access the Power BI file to see the report](https://drive.google.com/drive/u/0/folders/1f_SQIzkPXoSzGpK8hamR1k-LrN9pKODr)


### Result
<p>This project helped to gain knowledge on different tools like MS Power BI and different statistical methods to gain insights.With the above insight will help the client to understand the relationship between car features, pricing, and market categories to maximize profitability.
</p>
