# Alternative ML Model and the Evaluation of Strategy Returns

## Introduction:

The evaluation report aims to assess the performance of a trading algorithm over a period of six years using different parameters. The algorithm was tested on a standardized dataset, and the results were evaluated based on the cumulative product of actual returns versus strategy returns. The report focuses on the impact of changing the training window size and the Simple Moving Average (SMA) input features on the trading algorithm returns. Additionally, the report evaluates the effectiveness of the Logistic Regression model in improving the trading algorithm returns.

## Methodology:

The trading algorithm was tested using different parameter settings, including the size of the training dataset, the SMA input features, and the use of a Logistic Regression model. The impact of each parameter setting was recorded, and the best performing parameter setting was identified.



## Tune the Baseline Trading Algorithm

![Alt text]("actual_vs_strategy_returns_base.png")


## Changing the training window size:
The impact of increasing the training window size from 3 months to 6 months was evaluated. The results showed that the trading algorithm outperformed the actual returns with 1.8x compared to 1.6x. Therefore, increasing the training window size improved the performance of the trading algorithm.

![Alt text]("actual_vs_strategy_returns_Tune.png")

The size of the training dataset is a critical factor in machine learning model performance. Increasing the training dataset size can provide more historical data for the model to learn from but may result in overfitting. Conversely, decreasing the training dataset size may prevent overfitting but can result in the model not learning enough. The impact of changing the training window depends on the dataset and model. Finding the optimal training dataset size requires a balanced approach.

## Changing the SMA input features:
The SMA short window was increased from 4 to 6, and the SMA long window was increased from 100 to 120, keeping the 3-month time frame the same. The results showed that the actual returns performed better than the trading algorithm returns with 1.6x compared to 1.5x. Therefore, changing the SMA input features did not improve the performance of the trading algorithm.

![Alt text]("actual_vs_strategy_returns_SMAinputfeatures.png")

Adjusting the SMA input features can impact the model's signal reliability and quantity. Increasing SMA windows generates fewer, but more reliable signals, while decreasing SMA windows generates more signals but less reliably. The impact depends on the dataset and model. Optimal SMA window sizes should balance signal reliability and quantity. Decisions should align with model goals and dataset characteristics for enhanced performance and profitability.

## The best set of parameters: 

To find the best set of parameters for my trading algorithm, I conducted a series of tests. During these tests, I changed the time frame to 3, 6, and 12 months while simultaneously adjusting the SMA input features. Specifically, I experimented with changing the SMA fast window size from 4 to 5 and 6 and the SMA slow window size from 100 to 110 and 120.

However, I found that the optimal parameters depended on the specific dataset and model being used. Therefore, I emphasized the importance of conducting a systematic approach to parameter tuning by testing different parameter combinations to identify the best-performing set of parameters.

My experimentation revealed that 12 months was not a good choice for the time frame size, likely due to the size of the database. Ultimately, I found that the original parameters, which included a SMA fast of 4, SMA slow of 100, and a 3-month time period, provided the best results. These parameters outperformed the other parameters tested, including changes to the training window size and SMA input features.

In conclusion, my comprehensive testing and analysis highlight the importance of systematic parameter tuning to identify the optimal set of parameters for the specific dataset and model being used. My findings also demonstrate that the original parameters can provide the best results for this particular trading algorithm.

![Alt text]("actual_vs_strategy_returns_base.png")


## LogisticRegression model:

The LogisticRegression model was used to improve the performance of the trading algorithm. The results showed that the LogisticRegression model outperformed the other models tested. However, the original trading algorithm with the best set of parameters provided the highest returns.

![Alt text]("actual_vs_strategy_returns 4.png")






