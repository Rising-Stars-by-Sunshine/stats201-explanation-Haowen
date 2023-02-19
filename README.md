# PS2: Explanation
## Table of Contents

| Contents| URL |
| :---         |     :---     |
| Data | https://github.com/Rising-Stars-by-Sunshine/stats201-explanation-Haowen/tree/main/data |
| Code | https://github.com/Rising-Stars-by-Sunshine/stats201-explanation-Haowen/tree/main/code |
| Spotlight | https://github.com/Rising-Stars-by-Sunshine/stats201-explanation-Haowen/tree/main/spotlight |

## Data
### Data Source: 
- [Queried Data](https://github.com/Rising-Stars-by-Sunshine/stats201-prediction-Haowen/tree/main/data/Queried_Data)
- [Processed Data](https://github.com/Rising-Stars-by-Sunshine/stats201-prediction-Haowen/tree/main/data/Processed_data)

### Meta Data Information
| Data files| Data Content | Type|
| :---         |     :---     | :---: |
| ETHUSD.csv | Ethereum historical data from 2015 to 2021 | queried data |
| Ethereum_value.csv | Ethereum data after preprocessing | queried data |
| Regression_Train.csv | Data for model training | processed data |
| Regression_Test.csv | Data for model test | processed data |

### Data Dictionary 
| variable name | description | frequency     |  unit.    | range| type|
| :---         |     :---     |          ---: |---:        |---: |---: |
| Date | Represents the date at which the share is traded in the stock market | monthly |day|from 2015-08-07 to 2021-10-20|Object|
| Open | Represents the opening price of the stock at a particular date, which is the price at which a stock started trading when the opening bell rang | monthly |USD|from 0.431589 to 4174.635742|Numeric Types: float|
| Close | Represents the closing price of the stock at a particular date, which is the last buy-sell order executed between two traders. The closing price is the raw price, which is just the cash value of the last transacted price before the market closes | monthly |USD|from 0.434829 to 4168.701172|Numeric Types: float|



## Code
- [Query Ethereum Data](https://github.com/Rising-Stars-by-Sunshine/stats201-prediction-Haowen/blob/main/code/Query_Data_Ethereum_Data.ipynb)
- [Process Regression Data](https://github.com/Rising-Stars-by-Sunshine/stats201-prediction-Haowen/blob/main/code/Process_Data_Prepare_X_and_Y_for_Regressions.ipynb)
- [Analyze Data](https://github.com/Rising-Stars-by-Sunshine/stats201-prediction-Haowen/blob/main/code/Analyze_Data_Machine_Learning_for_Predicting.ipynb)
### Table of Code
| Code files| Description | Type|
| :---         |     :---:     | ---: |
| Query_Data_Ethereum_Data.ipynb  | This code deals with the read and preprocessing of the original dataset | .ipynb |
| Process_Data_Prepare_X_and_Y_for_Regressions.ipynb | This code processed the X and Y dataset from Ethereum_value.csv for regression  | .ipynb |
| Analyze_Data_Machine_Learning_for_Predicting.ipynb | This code applied machine learning method for open price regression| .ipynb |

## Spotlight
![image](https://github.com/Rising-Stars-by-Sunshine/stats201-prediction-Haowen/blob/main/spotlight/figures/Linear_Regression_Result.png)
*Figure 1: The prediction result of ethereum open price by linear regression*
- [Code source](https://github.com/Rising-Stars-by-Sunshine/stats201-prediction-Haowen/blob/main/code/Analyze_Data_Machine_Learning_for_Predicting.ipynb)
- [Data source](https://github.com/Rising-Stars-by-Sunshine/stats201-prediction-Haowen/tree/main/data/Processed_data)
- Description: from figure 1, it is obvious that the predicted result is very close to the real open price value. The result is evaluated by R2 score, which is 0.984. The R-squre determines the proportion of variance, which shows how well the data fit the regression mode(Chicco, Warrens, and Jurman 2021). The closer the r-squared value is to 1, the better the fit. Thus, the linear regression reached a high accuracy regarding the r-squared value.

# References

## Data Source
- [Ethereum Historical Dataset](https://www.kaggle.com/datasets/abhimaneukj/ethereum-historical-dataset)
## Code Source
- [Rising-Stars-by-Sunshine/stats201-tutorial-prediction](https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction/tree/main/code)
## Articles
- [Predicting Price Changes in Ethereum](https://cs229.stanford.edu/proj2017/final-reports/5244039.pdf)
- [The Coefficient of Determination R-Squared Is More Informative than SMAPE, MAE, MAPE, MSE and RMSE in Regression Analysis Evaluation](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8279135/)
## Literature
Chen, Matthew, Neha Narwal, and Mila Schultz. 2019. “Predicting Price Changes in Ethereum.” *International Journal on Computer Science and Engineering (IJCSE) ISSN*: 0975-3397.

Chicco, Davide, Matthijs J. Warrens, and Giuseppe Jurman. 2021. “The Coefficient of Determination R-Squared Is More Informative than SMAPE, MAE, MAPE, MSE and RMSE in Regression Analysis Evaluation.” PeerJ Computer Science 7 (July): e623. https://doi.org/10.7717/peerj-cs.623.

Zhang, Luyao (Sunshine). 2022. “Machine Learning for Predictions.” Machine Learning for Social Science, November. https://ms.pubpub.org/pub/ml-prediction/release/4.
