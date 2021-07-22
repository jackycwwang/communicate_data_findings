# The Factors for Prosper Loan Borrower's Interest Rate
## by Jacky Wang


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. Twelve promising features are chosen to do the analysis. Outliers were trimmed leaving 56,639 loans in the dataset so as to having a more generalized outcome. The original dataset can be found [here]( https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv)

In this investigation, my main focus would be interested in knowing what factors contribute to the decision of borrower's interest rate for the Prosper loan applications.

## Summary of Findings

From this investigation, I found that the most impactful numeric variable on the interest rate tends to be the borrower's credit score, which is a negative correlation; however, the variation of interest rate is quite large from score to score. The other numeric variables that have less influences are: loan amount, monthly payment, and number of investors. They all are negatively correlated with the interest rate. 

I also looked at three different categorical variables: Term, ProsperScore, and ProsperRating. It turns out that ProsperRating has the most clear and consistent representation in terms of less variation and clear trends; with higher the rating, lower the interest rate. The exploration shows that the categorical variable ProsperScore plays as a second place in deciding the interest rate with larger variation than ProsperRating.

Originally, I expected the loaning Term should have been an important factor. However, the risk scores dominate the term selection when the either risk is higher than certain threshold.


## Key Insights for Presentation

After exploration and analysis, I chose to shown only the most promising findings in the given dataset to answer my research question, which is the factors that influence the interest rate decision most. 

In the presentation, First, I chose to present the distribution of 2 most important variables: the interest rate and the borrower's credit score. Both of them appear closely to normal distribution, which is within expectation. Then, I showed the interaction between these two numeric variables using a scatter plot with a linear regression line to clearly indicate their negative correlation. After that, I went ahead to present the relationships beween the interest rate and the each of the three categorical variables using three violin plots. These plots clearly show the different degree of increase of the interest rate with each variable, being the ProsperRating the winner.

At the end, I brought in two point plots with two different categorical variabls and the interest rate. The trend is aligned with the violin plots. However, these plots also show an interesting finding that the positive correlation between term and the interest rate stops when the either risk is beyond certain limits. This clears my thought that loaning term should be one of the important factor. And it doesn't becuase the risk analysis dominates the term selection.