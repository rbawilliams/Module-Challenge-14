# Module-Challenge-14

![Alt text]("14-challenge-image.png")

## Answers 

Step 1: When increasing the size of the training dataset, the model has more historical data to learn from and may be able to better capture patterns and trends. However, a larger training dataset can also result in overfitting, where the model becomes too tailored to the specific training data and does not generalize well to new data. Conversely, decreasing the size of the training dataset may help prevent overfitting, but may result in the model not learning enough patterns and trends from the historical data. The impact of increasing or decreasing the training window will depend on the specific dataset and model being used.

Step 2: Adjusting the SMA input features can impact the model's ability to detect trends and generate signals. Increasing the SMA windows may result in fewer signals being generated, but those signals may be more reliable as they are based on a longer-term trend. Conversely, decreasing the SMA windows may result in more signals being generated, but those signals may be less reliable as they are based on shorter-term trends. The impact of adjusting the SMA input features will depend on the specific dataset and model being used.

Step 3: The set of parameters that best improves the trading algorithm returns will depend on the specific dataset and model being used. It is important to evaluate the cumulative product of the actual returns vs. the strategy returns for each set of parameters being tested, and choose the set of parameters that results in the highest cumulative product. This should be documented in the README.md file, along with the reasoning behind the parameter choices.