R Problem
We will analyze the relationship between diKerent personal attributes and medical
insurance charges using linear regression techniques.
Dataset
The Medical Insurance Cost dataset (`medical_cost.csv`) contains information about
individuals’ demographics, lifestyle factors, and their corresponding medical insurance
charges. This dataset is originally from the book Machine Learning with R by Brett Lantz.
Each row in the dataset represents an individual and includes the following attributes:
- `age`: Age of the individual.
- `sex`: Gender (`male` or `female`).
- `bmi`: Body Mass Index, a measure of body fat based on height and weight.
- `children`: Number of children/dependents covered by the insurance.
- `smoker`: Smoking status (`yes` or `no`).
STA 35B Winter 2025
- `region`: Residential area in the U.S. (`northeast`, `northwest`, `southeast`,
`southwest`).
- `charges`: The total medical insurance cost billed to the individual
Import `medical_cost.csv` onto R with the following name: `insurance`
R Question 1
a. Data Visualization: Create a scatter plot with `bmi` on the x-axis and `charges` on
the y-axis.
b. Correlation Estimation: Based on the scatter plot, estimate the correlation
coeKicient (r) between `bmi` and `charges`.
R Question 2
a. Linear Regression and Prediction: Fit a linear regression model to predict charges
based on `bmi`. Overlay the regression line on the scatter plot. Predict charges for
a person with a `bmi`of 30. Add the prediction point on the scatter plot with a
diKerent color.
b. Model Evaluation: Consider the scatter plot you produced. Is linear regression
appropriate for this data? Are any potential non-linearity and outliers observed?
c. Standardization and Visualization: Create a scatter plot with `bmi` and `charges`
in standard units and add predicted `charges` with using the linear regression
model. The color of the dots of the real and predicted values should be diKerent.
d. Comparison of Plots: Compare the scatter plots from original units (2.a) and
standardized units (2.c). Discuss similarities and diKerences.
R Question 3
a. Root Mean Squared Error (RMSE) Function: Define a function `rmse()` to compute
the Root Mean Squared Error (RMSE).
b. Optimization of Regression Parameters: Find the optimal slope and intercept that
minimize RMSE. Overlay the optimized regression line on the scatter plot.
c. Justification of Optimization Approach: Why does minimizing RMSE lead to the best-
fit regression line? Discuss the relationship between RMSE and least squares
regression.
d. Alternative Error Metrics: Which of the following error metrics would yield the same
slope and intercept as RMSE?
1. ∑ |𝑒! |"
!#$
2. ∑ 𝑒!
%"
!#$
STA 35B Winter 2025
3. $
" ∑ |𝑒! |"
!#$
4. $
" ∑ 𝑒!
%"
!#$
R Question 4
Exploring Another Relationship
a. Create a scatter plot of age vs. charges and fit a regression line. Overlay the
regression line over the scatter plot.
b. Assuming linear regression is a reasonable model, indicate whether the following
statements are true or false. Explain your reasoning.
1. The regression line suggests that older individuals tend to have higher
medical charges on average.
2. There is a clear and strong linear relationship between age and medical
charges.
3. The data shows multiple clusters of points, indicating that age alone may not
fully explain medical charges.
4. A randomly selected individual with an age of 40 will always have a medical
charge close to the regression line’s prediction.
5. If we standardize both age and medical charges, the regression line will still
have the same correlation coeKicient.
6. Since the regression line is slightly increasing, it suggests that increasing age
causes higher medical expenses.
7. If an individual has the same age as another but much higher charges, the
model may not accurately predict their medical costs.
8. The spread of data points suggests that there are other important variables
influencing medical charges.
