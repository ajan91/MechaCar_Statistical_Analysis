# MechaCar_Statistical_Analysis

# Background + Overview

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes

- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots

- Run t-tests to determine if the manufacturing lots are statistically different from the mean population

- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

**Deliverables**
This assignment consists of three technical analysis deliverables and a proposal for further statistical study.

Deliverable 1: Linear Regression to Predict MPG
Deliverable 2: Summary Statistics on Suspension Coils
Deliverable 3: T-Test on Suspension Coils
Deliverable 4: Design a Study Comparing the MechaCar to the Competition

# Deliverables

**Deliverable 1: Linear Regression to Predict MPG**
Deliverable 1 Requirements

You will earn a perfect score for Deliverable 1 by completing all requirements below:

- The MechaCar_mpg.csv file is imported and read into a dataframe (5 pt)

- An RScript is written for a linear regression model to be performed on all six variables (10 pt)

- An RScript is written to create the statistical summary of the linear regression model with the intended p-values (10 pt)

- There is a summary that addresses all three questions (5 pt)


The image above shows that vehicle length, vehicle ground clearance 

The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. The vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.

The p-Value for this model, p-Value: 5.35e-11, is much than the assumed significance level of 0.05%.

This linear model has an r-squared value of 0.7149, which means that 71% of all mpg predictions will be determined by this model. Relatively speaking, his multiple regression model does predict mpg of MechaCar prototypes effectively.

If we remove the less impactful independent variables the predictability does decrease: the r-squared value falls from 0.7149 to 0.674.

**Deliverable 2: Create Visualizations for the Trip Analysis**
Deliverable 2 Requirements

- The Suspension_Coil.csv file is imported and read into a dataframe (5 pt)

- An RScript is written to create a total summary dataframe that has the mean, median, variance, and standard deviation of the PSI for all manufacturing lots (10 pt)

- An RScript is written to create a lot summary dataframe that has the mean, median, variance, and standard deviation for each manufacturing lot (10 pt)

- There is a summary that addresses the design specification requirement for all the manufacturing lots and each lot individually (5 pt)

**Deliverable 3: T-Tests on Suspension Coils**
Deliverable 3 Requirements

- An RScript is written for t-test that compares all manufacturing lots against mean PSI of the population (5 pt)
- An RScript is written for three t-tests that compare each manufacturing lot against mean PSI of the population (10 pt)


- There is a summary of the t-test results across all manufacturing lots and for each lot (5 pt)
The true mean of the sample is 1498.78, which we also saw in the summary statistics above. With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis. In other words, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.

**Deliverable 4 Requirements**
Deliverable 4 Requirements

The statistical study design has the following:

**A metric to be tested is mentioned (5 pt)** 
- Safety Feature Rating: Independent Variable
- Current Price (Selling): Dependent Variable
- Drive Package : Independent Variable
- Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
- Resale Value: Independent Variable
- Average Annual Cost of ownership (Maintenance): Independent Variable
- MPG (Gasoline Efficiency): Independent Variable

**A null hypothesis or an alternative hypothesis is described (5 pt)**
- Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
- Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.

**A statistical test is described to test the hypothesis (5 pt)**
**The data for the statistical test is described (5 pt)**

A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price.
