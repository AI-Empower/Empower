# RQ1 - How do the AI models compare in terms of accuracy in solving math problems?

1. **Comparative Accuracy Analysis**: How do the AI models compare in terms of accuracy in solving math problems?
   - **Analysis Method**: Chi-Square Test.
   - **Rationale**: This test is suitable for categorical data (correct/incorrect) to compare the frequencies of correct answers across different models.
   - **Assumptions**: Independence of observations, expected frequency in each cell ≥ 5.

-- SEE THE END FOR THE UPDATED RUN WITH A 50% SAMPLE SIZE INCREASE! --

### Data Preparation for Analysis

1. **Chi-Square Test**: We'll aggregate the data to compare the number of correct and incorrect answers for each model.

```
from scipy.stats import chi2_contingency

# Preparing data for the Chi-Square Test
# Counting the number of correct and incorrect answers for each model
chi_square_data = data.groupby('Model')['Zero-Shot Accuracy as Correct (1 for Yes, 0 for No)'].value_counts().unstack()

# Conducting the Chi-Square Test
chi2, p, dof, expected = chi2_contingency(chi_square_data)

# Displaying the contingency table and the results of the Chi-Square Test
chi_square_data, {'Chi-Square Statistic': chi2, 'p-value': p, 'Degrees of Freedom': dof, 'Expected Frequencies': expected}
```

The Chi-Square test yields the following results:

- **Chi-Square Statistic**: 8.88
- **p-value**: 0.0118
- **Degrees of Freedom**: 2
- **Expected Frequencies**:
  - Bard: Incorrect (3.33), Correct (16.67)
  - GPT3.5: Incorrect (3.33), Correct (16.67)
  - GPT4: Incorrect (3.33), Correct (16.67)

### Interpretation
- The **Chi-Square Statistic** of 8.88 and a **p-value** of 0.0118 suggests that there is a statistically significant difference in the accuracy of the AI models (Bard, GPT3.5, and GPT4) when solving math problems.
- The **p-value** (0.0118) is less than the typical alpha level of 0.05, indicating that the observed differences in model performance are unlikely to be due to chance.
- The **Expected Frequencies** suggest what the distribution of correct and incorrect answers would look like if there were no difference between the models' performance. The actual data deviates from these expectations, particularly for GPT4, which outperforms the other models with zero incorrect answers.

This analysis answers the first research question, demonstrating significant differences in performance among the AI models. For the remaining research questions, additional data processing would be required, such as categorizing math problems for logistic regression or calculating problem complexity for correlation analysis.

Analysis Code
```
# Filling missing values with 0 for the Chi-Square Test
chi_square_data_filled = chi_square_data.fillna(0)

# Conducting the Chi-Square Test again with the adjusted data
chi2_filled, p_filled, dof_filled, expected_filled = chi2_contingency(chi_square_data_filled)

# Displaying the adjusted contingency table and the results of the Chi-Square Test
chi_square_data_filled, {'Chi-Square Statistic': chi2_filled, 'p-value': p_filled, 'Degrees of Freedom': dof_filled, 'Expected Frequencies': expected_filled}
```
# Concerns Remained 
## A balance between independant researcher capability & robust data must be struck
So I increased my sample size by 50%
## The Chi-Squared test - Take 2 
*Those results have been provided below in an abbreviated form:*

#### Contingency Table
```
Zero-Shot Accuracy as Correct ( Correct = 1, Incorrect = 0)  0.0  1.0
Model                                                                
Bard                                                           9   21
GPT3.5                                                         5   25
GPT4                                                           0   30
```

#### Test Results
- Chi-Squared Statistic: 10.32
- Degrees of Freedom: 2
- p-value: 0.00574
- Expected Frequencies:
```
[[ 4.66666667 25.33333333]
 [ 4.66666667 25.33333333]
 [ 4.66666667 25.33333333]]
```

### Conclusion

Based on the p-value of 0.00574, we can conclude that there is a statistically significant difference in accuracy among the three AI models. This suggests that not all models perform equally in terms of accuracy on the given dataset.
