# Machine Learning Trading Bot

![Alt text](14-challenge-image.png)

## Overview
This project involves creating an algorithmic trading bot that can learn and adapt to new data and evolving markets. As a financial advisor at one of the top five financial advisory firms in the world, my goal is to maintain our firm's competitive advantage while providing the best possible returns for our clients. I plan to enhance the existing algorithmic trading systems by using machine learning algorithms that can adapt to new data.

## Background
In recent years, algorithmic trading has become increasingly popular in the financial industry. Algorithmic trading systems can process large amounts of data in real-time, allowing traders to make faster and more informed trading decisions. However, these systems are only as good as the algorithms that power them. As markets become more complex and unpredictable, traditional trading algorithms can struggle to keep up.
To address this challenge, machine learning algorithms can be used to enhance algorithmic trading systems. Machine learning algorithms can learn and adapt to new data, allowing them to make more accurate predictions about market trends and price movements. In this project, I will use historical stock data to train a machine learning classifier that can predict whether to buy or sell a stock.
In this project, I use historical stock data to train a machine learning classifier that can predict whether to buy or sell a stock. Specifically, I generated trading signals using short- and long-window simple moving averages (SMA) and use the support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data.

## Methodology:

### Data Preparation:
- Import OHLCV dataset into a Pandas DataFrame.
- Generate trading signals using short- and long-window SMA values.
### Data Split:
- Split the data into training and testing datasets.

### Modeling:
- Use the SVC classifier model from SKLearn's SVM learning method to fit the training data and make predictions based on the testing data.
- Review the predictions.
- Review the classification report associated with the SVC model predictions.
- Create a predictions DataFrame that contains columns for "Predicted" values, "Actual Returns", and "Strategy Returns".
- Create a cumulative return plot that shows the actual returns vs. the strategy returns.

### Tuning:
- Adjust the size of the training dataset by slicing the data into different periods and rerun the notebook with updated parameters.
- Adjust one or both of the SMA input features and rerun the notebook with updated parameters.

## Conclusion:
In conclusion, the GitHub repository presents a comprehensive evaluation of a trading algorithm's performance over six years, considering different parameters such as the training dataset size, SMA input features, and time frame. Through a series of tests and experiments, the best-performing set of parameters was identified, highlighting the critical role of systematic parameter tuning in developing an effective trading algorithm. 
The findings suggest that increasing the training window size enhances the algorithm's performance, whereas changing the SMA input features does not yield any significant improvement. Additionally, the report evaluates the effectiveness of using a LogisticRegression model in enhancing the algorithm's performance, with the original algorithm's best-performing set of parameters providing the highest returns. The report's insights emphasize the importance of achieving a balance between the parameters to optimize the algorithm's performance and can guide future research and development of trading algorithms, ultimately resulting in improved performance and profitability.

## License
The code in this project is licensed under the MIT License.