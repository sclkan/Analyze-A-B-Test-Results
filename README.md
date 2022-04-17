# Analyze A/B Test Results
Our client, an e-commerce company, has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product.

We will perform an A/B test to understand if they should implement the new page design or keep the old one.  In addition, we will apply other statistical methods such as probability and logistic regression to help cross-check our results.

## Results
[Analyze_ab_test_results_notebook.ipynb](https://github.com/sclkan/Analyze-A-B-Test-Results/blob/master/Analyze_ab_test_results_notebook.ipynb)

## Summary
We have used probabilities, hypothesis testing, and logistic regression to help determine whether the new web page can increase the conversion rate. All three methods imply that the new page design does not have any significant effect on conversions. A detailed summary of the results is as follows:

- Probability: The difference in converted rate between the two designs is -0.001578, which means there isn't sufficient evidence to infer that the new page will lead to more purchases.
- A/B Test: P-value = 0.906 with an α of 5%. We fail to reject H0, which suggests that the difference between the two pages is not statistically significant. In other words, the new page design does not yield higher conversions.
- Logistic Regression: P-value = 0.19 with an α of 5%. The result indicates that the page design alone is not statistically significant enough in predicting the conversion rate. Even if we incorporate another variable such as countries to the same regression model, p-values are still considerably larger than 0.05; there is no evidence that page design has any effect on conversions.


## Source
*ab_data.csv* and *countries.csv* provided by Udacity

## Python Libraries
Pandas, NumPy, Matplotlib, Statsmodels
