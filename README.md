# AN-ANALYSIS-OF-CLIMATE-CHANGE-BELIEFS-USA-ON-DEMOGRAPHICS-AND-OTHER-SOCIO-ECONOMIC-FACTORS
Public opinion about global warming is an important influence on decision making about policies to reduce global warming or prepare for the impacts, but We can't get people to vote for adopting the policies unless people believe that Global Warming is happening and Global Warming is caused mostly by human activities. But American opinions vary widely depending on where people live, our project is based on the Yale climate opinion maps-2016 surveys outcome where 18,000 American people survey response was recorded about opinion on climate change 7 in 10 American   believes that global warming is happening. the study conducted by Yale was based on certain set of question being asked and people got surveyed on the basis of metro cities, counties and state wise, the outcome of the opinion survey is result of some statistical models. for our further study where we wanted to know that what are demographic factors like race, age ,sex and income, ,education level of people who believes or in favor of global warming happening and people who oppose the idea of global warming. To carry out this study we combine us-census -demographic data.   And we also added more factors like temperature anomalies by counties from noaa.gov. After combining the data sets from different sources which was a  huge task  we ran model in SAS MINER ran model regression and  neural network and got outcome like Race (Asian, White, Hispanic believes more), Gender (men believe less),Education (people with bachelor’s degrees believe more),Community type (rural people believe less), Average temp anomaly, precipitation anomaly, precipitation inches are important factor and where government and people's individual efforts work better to fight bad effects of climate change.
![image](https://user-images.githubusercontent.com/59974486/90712468-1afa1400-e271-11ea-8d78-9c98d1d7e13f.png)

METHODOLOGY
SAS Enterprise Miner was used to analyze the climate change dataset. For believer and non-believer classification, we build decision tree and neural network models with all demographics and temperature inputs then picked the model with lower misclassification rate. 
For climate change beliefs prediction, we have four target variables that needs to be predicted based on the demographics, socio-economic and temperature variables at county level. The target variables include percentage of people believe global warming is happening,  percentage of people believe that  global warming is NOT happening, percentage of people believe that global warming is caused mostly by human activities and percentage of people believe that global warming is NOT caused by human activities. We applied the same methodology for each of the target variable as follows. We first built a Regression model to study which inputs variables play more important roles in predicting the target variable based on p-values. Next, we built the first Neural Network with the input variables solely chosen by Variable Selection tool. Variable Section tool selected variables based on R-squared. Rejecting the input variables that have low R-squared scores helps to reduce the number of input variables to analyze in the first Neural Network model. After that, we built a second Neural Network model with the input variables manually selected based on both p-value (from Regression model) and R-squared (from Variable Selection model). Lastly, we chose the best model from the three by comparing the MSE values on the test dataset.

![image](https://user-images.githubusercontent.com/59974486/90774933-34797b00-e2c6-11ea-9a37-90ce6090e10f.png)
