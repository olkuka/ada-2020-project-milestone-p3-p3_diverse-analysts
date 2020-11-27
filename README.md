# ada-2020-project-milestone-p3-p3_diverse-analysts

1. **Title** 

Predicting NYC property sales with Google Trends

2. **Abstract**

    In our assigned paper there are explored different datasets by analyzing how Google Trends data could influence economic predictions such as initial claims for unemployment, automobile demand and vacation destinations. We propose to examine a different dataset related to the NYC sales property and check how Google Trends data impact the prediction. 


    To do so, we will find out several Google Trends categories and analyze which are better to improve the model. So, we will execute the autoregressive model, setting out different possibile lags and observe if using Google Trends has a positive effect both on the in-sample fit and out-of-sample forecasting. Indeed, we will compute the MAE, examining if it will be meliorate or not and, finally we will plot the actual log of the sales and the ones we obtained with and without Trends, in order to understand better Google Trends effect. Furthermore, we will search for possible turning points (e.g. 2016 election in the US) in the time series and in that case we will report the different MAE around turning points, finding out in which exact periods Google Trends fits better than the Base model.  

3. **Research questions**
*   Which categories should we choose to improve prediction?
*   Do the chosen categories improve in-sample fit?
*   Do the chosen categories improve out-of-sample forecasting?
*   Do we see an improvement in MAE?
*   Is there a correlation between a higher number of searches for properties category on Google Trends in NYC and the actual number of sold flats?
*   Did the election of Donald Trump in November 2016 have any effect on the sales?
4. **Proposed datasets**
* nyc-rolling-sales.csv from the “NYC property sales” Kaggle dataset [nyc!](https://www.kaggle.com/new-york-city/nyc-property-sales)
* google trends data regarding properties, apartments searches in the area of New York / New York state
5. **Methods**
*   Data collection: use gtab (GoogleTrendsAnchorBank) library to extract required data from Google Trends, download the dataset from Kaggle. Substitute mising values if such exist with meaningful data (similar to HW2). Lastly, select all necessary features for our analysis.
*   Data analysis: construct Autoregressive Model using Statsmodels, compare the improvement with respect to the base model based on the MAE (experiment with different Google queries, lags) 
*   Visualization: plot the differences using Seaborn, reflect on any turning points if such exist. Mark 2016 US Election day on the plot.
6. **Proposed timeline**

**Week 1**: downloading and exploring the NYC sales property dataset from Kaggle. Selecting only the columns useful for our scope and moving forward with data cleaning and preprocessing. Searching via Google Trends for different categories that could have an impact on the prediction. Downloading the query index data as a CSV file.

**Week 2**: implementing the autoregressive model, trying different lags for figuring out the better ones. Fitting firstly the model with Base data, then add Google Trends categories looking at their effect in-sample forecasting and also out-of-sample. Computing MAE. Data analysis and data visualization of the obtained results, with and without Trends.

**Week 3**: Completing data analysis. Setting up our conclusion and carrying out the data story. Realization of the final video.



7. **Organization within the team**
*   Bartłomiej had already downloaded the NYC sales property dataset from Kaggle. He did basic data cleaning and data preprocessing also. Then he shared his notebook and the whole team met to explore the data together and think about research questions.
*   In week 1, Aleksandra will be searching the possible matching categories in Google Trends. Together with Bartłomiej, they will try to use Google Trends Anchor Bank created by dlab to crawl Google Trends. Meanwhile, the dataset will be fully reviewed by all team members and Bartlomiej will finish data preprocessing by selecting the required features and dealing with missing values (if such exist in the datasets).
*   In week 2, Diana will  implement the autoregressive model with lags that suits the best. In collaboration with Aleksandra, they will together try to choose the categories which improve the prediction. They will be computing Mean Absolute Errors, creating visualizations, so they can compare the results and choose the best categories. At the end of week 2 the data analysis will be done. During this whole week, Bartłomiej will be writing a corresponding data story. 
*   In week 3, the whole team will make sure that everything is right and, after that, Bartłomiej will start to create a short video. Diana and Aleksandra will be working on visualizations of the data story which may be shown in the video as well. 
8. **Questions for TA (optional)**
