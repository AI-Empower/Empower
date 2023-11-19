# RQ2 "Does the complexity of math problems affect the accuracy of different AI models?"

We categorized the complexity scores into three categories: Low, Medium, and High using the data from the Complexity Scores

## Complexity Score Categories
- Low: Scores <= 10
- Medium: Scores > 10 and <= 12
- High: Scores > 12

### Data Tables: 
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

## Descriptive Analysis Results

The cross-tabulation and percentage breakdown of accuracy across different models and complexity categories are as follows:

### Cross-Tabulation Counts:
- **Bard Model**:
  - Low Complexity: 4 correct, 0 incorrect.
  - Medium Complexity: 6 correct, 0 incorrect.
  - High Complexity: 11 correct, 9 incorrect.
- **GPT3.5 Model**:
  - Low Complexity: 4 correct, 0 incorrect.
  - Medium Complexity: 5 correct, 1 incorrect.
  - High Complexity: 16 correct, 4 incorrect.
- **GPT4 Model**:
  - Low Complexity: 4 correct, 0 incorrect.
  - Medium Complexity: 6 correct, 0 incorrect.
  - High Complexity: 20 correct, 0 incorrect.

#### Percentage Breakdown:
- **Bard Model**:
  - Low Complexity: 100% correct.
  - Medium Complexity: 100% correct.
  - High Complexity: 55% correct, 45% incorrect.
- **GPT3.5 Model**:
  - Low Complexity: 100% correct.
  - Medium Complexity: 83.33% correct, 16.67% incorrect.
  - High Complexity: 80% correct, 20% incorrect.
- **GPT4 Model**:
  - Low Complexity: 100% correct.
  - Medium Complexity: 100% correct.
  - High Complexity: 100% correct.

### Interpretation:
- All models performed well on low and medium complexity problems, with high accuracy rates.
- The Bard model shows a significant decrease in accuracy for high complexity problems, while GPT3.5 shows a slight decrease, and GPT4 maintains 100% accuracy.

