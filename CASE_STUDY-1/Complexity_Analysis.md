# RQ2 "Does the complexity of math problems affect the accuracy of different AI models?"

We categorized the complexity scores into three categories: Low, Medium, and High using the data from the Complexity Scores

### Complexity Score Categories
- Low: Scores <= 10
- Medium: Scores > 10 and <= 12
- High: Scores > 12

### Detailed Assumption Tables: 
```
Zero-Shot Accuracy as Correct ( Correct = 1, Incorrect = 0)  0.0  1.0
Model  Complexity Category                                           
Bard   High                                                    4    0
       Medium                                                  5   11
       Low                                                     0   10
GPT3.5 High                                                    2    2
       Medium                                                  2   14
       Low                                                     1    9
GPT4   High                                                    0    4
       Medium                                                  0   16
       Low                                                     0   10
```


### Interpretation:
- The chi-square statistic measures how much the observed frequencies differ from the expected frequencies. A higher value indicates a greater discrepancy.
- The p-value indicates the probability of observing a chi-square statistic as extreme as (or more extreme than) the observed value under the null hypothesis (which in this case is that there is no association between the complexity of math problems and the accuracy of different AI models).

Since the p-value (0.00922) is less than the conventional alpha level of 0.05, we reject the null hypothesis. This suggests that there is a statistically significant association between the complexity of math problems and the accuracy of different AI models.

### Caveats:
- The Chi-Square Test's assumption of expected frequencies being at least 5 in each cell was violated in several cases. This may affect the robustness of the results.
- The small sample size in some categories could also limit the generalizability of the findings.

### Conclusion:
Based on the analysis, it appears that the complexity of math problems does affect the accuracy of different AI models. However, due to limitations in the data (such as small expected frequencies in some categories), this conclusion should be considered with caution. Further research with a larger dataset and more evenly distributed responses across complexity levels would be beneficial to confirm these findings.
