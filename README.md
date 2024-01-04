<![Headerimage](./Charts%20%26%20Images/Image1.jpg)

# Analysis of House Sales in King County, WA

DSC Phase 2 Project

**Authors:** 
Group 17 - Caroline Mbugua, Diana Wangura, Mark Kuria, Rhoda Musyoki, Alice Jebiwott, Mlati Ochieng

## Overview

BuildKesho Consultancy Ltd is embarking on data-driven property analysis within the King County real estate market. Our focus is on developing a predictive model that forecasts house prices and identifies key property features influencing market valuation. This data-driven approach aims to empower our clients with insights for informed investment decisions.


## Business and Data Understanding

BuildKesho Consultancy Ltd aims to develop a predictive model that not only forecasts house prices but also identifies key property features influencing market valuation. This data-driven approach aims to empower clients with valuable insights, guiding them towards informed investment decisions. 

Our stakeholders include prospective homebuyers and investors seeking expert advice, ensuring they make sound choices in the competitive King County real estate landscape.  

The data source for this analysis is the King County House Sales dataset (kc_house_data.csv) which contains information about the price, location, size, condition and other features of houses sold in King County from January 2014 to December 2015. This dataset forms the basis for our predictive model, offering a robust foundation for analysis and decision-making.  

## Modelling

A multiple linear regression model was designed using selected features such as 'bedrooms', 'bathrooms', 'sqft_living', 'sqft_lot' and others, with the house 'price' as the dependent variable.

OLS method was utilized to fit the model. This technique is standard in linear regression and works by minimizing the sum of the squared differences between observed and predicted values.

<![AvP](./Charts%20%26%20Images/Actual vs Predicted Prices.png)

Model Output Analysis:

- R-squared: The model achieved an R-squared value of 0.65. This means that 65% of the variation in house prices could be explained by the model’s independent variables.

- Coefficients: The model provided a coefficient for each independent variable, indicating its individual impact on the house price. For example, variables like 'bathrooms' and 'sqft_living' had a positive relationship with the price.

- P-values for each coefficient were checked to determine the statistical significance of the variables. 

The coefficients offered insights into how much each feature would, on average, impact the house price, holding other variables constant.
The intercept term in the model provided a baseline house price when all predictors are at zero.

Residuals were calculated as the difference between actual and predicted values and analyzed using scatter plots and histograms to check for any patterns or biases. A QQ plot was also used to test the normality of residuals.

<![Residualsplot](./Charts%20%26%20Images/Residuals.png)



## Regression Results

The multiple linear regression model was employed to predict house prices based on various independent variables. The model includes features such as bedrooms, bathrooms, square footage of living space, lot size, floors, year built, condition, grade and waterfront presence.

The results of the regression analysis are as follows:

R-squared: The model explains approximately 65% of the variance in house prices, indicating a good fit.

Coefficients:

- Bedrooms: Each additional bedroom decreases the estimated house value by $42,820
- Bathrooms: Each additional bathroom increases the estimated house value by $50,430
- Sqft_living: An increase in living space by one square foot increases the estimated value by $180
- Other coefficients for floors, condition, grade and waterfront presence are also significant


## Conclusion

In conclusion, the multiple regression model provides valuable insights into the factors influencing house prices in King County. The recommendations below, derived from the model can be utilized by potential homebuyers, investors and BuildKesho Consultancy Ltd to make informed decisions in the real estate market:

1. Stakeholders should prioritize understanding and enhancing grade score descriptions. Consideration of luxurious amenities, up-to-date building plans and meticulous attention to exterior and interior finishes can significantly contribute to increased home value.

2. Stakeholders are advised to prioritize properties with waterfront features to capitalize on the considerable estimated value boost

3. Where feasible, have additional bathrooms as this significantly boosts the estimated value of the house, with each extra bathroom contributing an increase of 50,430 USD

4. Increasing the living space of a home is associated with a positive impact on its estimated value. Consider renovation or expansion projects to capitalize on this potential value increase

5. If applicable, properties with multiple floors exhibit a higher estimated value. Exploring or investing in homes with multiple floors could be a worthwhile consideration.



## For More Information

See the full analysis in the [Project Jupyter Notebook](./dsc-phase2-project-notebook.ipynb) or review this [Project Presentation](./DSC-dsc-phase2-project-presentation.pdf)


## Repository Structure

```
├── Charts & Images
├── Data
├── dsc-phase2-project-notebook.ipynb
├── dsc-phase2-project-presentation.pdf
└── README.md
```
