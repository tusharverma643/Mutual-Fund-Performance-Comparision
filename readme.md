# Mutual Fund Performance Comparison

This Python script compares the performance of two mutual funds using a parametric t-test. It is designed to help you assess whether there is a statistically significant difference in the performance of two mutual funds over a specific period.

## Features

- Normality Check: The script first checks the normality of the data for both mutual funds using the Shapiro-Wilk test from the `scipy.stats` module. This step ensures that the data follows a normal distribution, which is a prerequisite for the t-test.

- Variance Homogeneity Check: Next, it examines whether the variances of the two samples are equal using Levene's test. This step is important because the t-test assumes equal variances in the samples.

- T-test for Comparison: After confirming that the assumptions are met, the script proceeds to perform a t-test for independent samples to compare the mean returns of the two mutual funds.

- Level of Confidence: The user can set the desired level of confidence for the t-test (e.g., 95% or 99%). The script will provide the results based on the chosen significance level.

## Dependencies

The following Python packages are used in this project:

- numpy
- pandas
- matplotlib
- scipy.stats

Make sure to install these packages before running the script.

## How to Use

1. Provide Data: Ensure that you have the historical returns data for both mutual funds. The data should be aligned correctly for the corresponding quarters or periods.

2. Configure Confidence Level: Set the desired level of confidence for the t-test in the script. For instance, if you want a 95% confidence level, set the `level_of_confidence` variable to 0.05.

3. Run the Script: Execute the Python script and follow the instructions in the terminal. The script will conduct the t-test and display the results.

## Practical Application

This script was developed during an internship to help determine whether a new mutual fund (e.g., Motilal Oswal MidCap fund) should be included in the investment offering. By comparing the performance of different funds using statistical tests, it helps to strike a balance between the brokerage received and the returns the funds provide. It allows for data-driven decision-making and provides valuable insights into the potential performance differences between different investment options.

Please note that past performance is not indicative of future results, and the decision to include or exclude a mutual fund should also consider other factors beyond statistical analysis.

## Disclaimer

This script is meant for educational and analytical purposes only. It does not provide financial advice or investment recommendations. Always consult a qualified financial advisor before making any investment decisions. The authors are not responsible for any financial losses or gains resulting from the use of this script.

## Author

Tushar Verma
