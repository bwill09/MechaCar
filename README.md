# MechaCar

### MechaCar Analysis 

### Overview of Project 

Jeremy begun a role and few weeks later senior management spoke to him about a special project, MechaCar, with production difficulties that prevents manufacturing team’s progress. So management asked Jeremy and their data team to review production data for opinion that could help the manufacturing team. 

### This project will support Jeremy and the data team with the following:

•	Run t- test to analyze the manufacturing statistics of lots 
•	Design studies statistically to match vehicle performance of the MechaCar vehicles against vehicles from other manufactures 
•	Summary statistics on pounds per square inch (PSI) of the suspension coils for the manufacturing lots 
•	Execute multiple linear regression analysis 


### Resources

*	Data Source: MechaCar_mpg.csv and Suspension_Coil.csv
*	Data Tools: tidyverse, dplyr, ggplot2 and MechaCarChallenge.RScript
*	Software: RStudio and R

### Deliverable 1

Linear Regression for MPG 

The MechaCar_mpg_csv dataset contains mpg data for portotype MechaCars. They were produce doing multiple design analysis to point out specific vehicle ability. Several scale, like vehicle weight, vehicle length and more were collected for each vehicle. 

Result on D1:

<img width="588" alt="p-Value" src="https://user-images.githubusercontent.com/106555873/190924136-b4aab0f0-a21b-46fa-a5d8-472da50b9341.png">

### Summary:

*		The p-Value of this model, P-Value: 5.35e-11, lower that .05%. This case indicates enough reason to reject our null hypothesis. Furtherance, this suggests that the slope of this linear model is not zero. 

*		The linear model has an r-squared value of 0.7149 which could sum up 71% of all mpg assumption by this model.

*		Vehicle length, and vehicle ground clearance can most likely produce non-random amounts of variance to the model. In other words, the vehicle length and vehicle ground clearance comprise of substantial hit on miles per gallon on the MechaCar prototype. Oppositely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicates arbitrary of variance with dataset

Summary Statistics (Suspension Coils)

Suspension Coil dataset contained the MechaCar results of testing the weight abilities of multiple suspension coils form multiple production lots to identify consistency 

### Result 1:

<img width="344" alt="1st lot" src="https://user-images.githubusercontent.com/106555873/190924190-35ced189-6c00-4879-95f4-9f5ca266c5b2.png">

<img width="493" alt="all lots png " src="https://user-images.githubusercontent.com/106555873/190924339-bbc8342a-8004-46e7-8c9a-681e9c19e7cc.png">

Given the fact based on design specs for the MechaCar suspension coils indicates that the variance of the suspension coils should not exceed 100 pounds per square inch (PSI)

Considering the whole population of the production lot, the variance is within the 100 PSI variance standard

Lot 1 and 2 within the 100 PSI variance requirement, with variance of 0.97 and 7.46. Lot 3 has bigger variance in performance and steadiness, with a variance of 170.28. Lot 3 excessively causing the variance at all the lot level

### T-tests on Suspension Coils 

<img width="769" alt="t-test" src="https://user-images.githubusercontent.com/106555873/190924371-8dd6f012-f2c8-4d26-aef9-b4fa60f5d2cd.png">

1.	Lot 1 has the true sample mean of 1500, in the summary statistics. With a p-Value of 1, clearly we cannot reject (i.e. accept) the null hypothesis that there is no statistical difference between the observed sample mean and the intended population mean (1500).
2.	Lot 2 has similar outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically alike.
3.	Lot 3, exhibits a different scenario. The sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.


Lot2

<img width="592" alt="Lot2" src="https://user-images.githubusercontent.com/106555873/190924458-47214680-52db-4cbc-a683-9b3264bcd21c.png">

Lot3 

<img width="593" alt="Lot 3" src="https://user-images.githubusercontent.com/106555873/190924461-22ad8984-f28d-41c6-8f7d-c45197bc8141.png">


### Deliverable 4

Study Design: MechaCar vs other competitors 

A study gathering data on MechaCar and its comparable models across multiple  manufacturers over 3 years.
*	What are comparable models for competitors 
*	Which cars will MechaCar be comparing with head-to-head? which cars will be included in the study?
*	Which elements would determine the selling price?

### Metrics

Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:
*	Safety Feature Rating: Independent Variable
*	Current Price (Selling): Dependent Variable
*	Drive Package : Independent Variable
*	Engine (Electric, Hybrid, Gasoline): Independent Variable
*	Resale Value: Independent Variable
*	Average Annual Cost of ownership (Maintenance): Independent Variable
*	MPG (fuel efficiency): Independent Variable

### Hypothesis: Null and Alternative

After looking at which factors are vital for the MechaCar's type:

*	Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its type.
*	Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.

### Statistical Tests

* A multiple linear regression would be used to identify elements that have the best predictability with the current selling price, which has the most influence on price
