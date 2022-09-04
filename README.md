<h1> Linear-Regression-Case-Study-Bike-Sharing </h1> 
Brief description of the project:

- BoomBikes have contacted a consulting company to understand the factors on which the demand for these shared bikes depends. 
Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market.

##The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.

- How well those variables describe the bike demands

- Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.


## General Information
- We are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. 
- They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.


### Final Conclusions
##Conclusion from Bike Sharing dataset EDA:
- Also it is quite clear that atemp is directly derived from temp and hence if atemp is taken into account, temp becomes redundant.
- The hiring rate is more for 2019 than 2018
- Fall shows a higher demand followed by summer season
- May to October period also shows a higher demand than other parts of the year
- working days are having a higher demand than holidays and weekends
- Clear weather days attract a hire demand then other days.
- Temperature is having a positive correlation(0.63) with demand. And higher temp attracts more bike hiring.
- Windspeed shows somewhat negative correlations(-0.24) with count.

##Model Building and Evaluation Conclusion:
- Final Equation for Prediction :
const * 0.2530 + yr * 0.2560 + holiday * -0.0544 + windspeed * -0.1670 + season_spring * -0.2023 + season_winter * 0.0350 + mnth_december * -0.1609 + mnth_february * -0.1027 + mnth_january * -0.1464 + mnth_november * -0.1491 + mnth_september * 0.0591 + weathersit_clear * 0.2909 + weathersit_moderate * 0.2008

- r2_score for train data set is 80%

- r2_score for test data set is 77.11%

- we used RFE for automatic feature elimation , after that we removed 'atemp','hum','mnth_july' based on p and VIF values

- based on trained model and our analysis, top three features contributing to shared bikes demand are yr, weather situation, september month.

## Technologies Used
- pandas - version 1.2.4
- numpy - version 1.20.1
- seaborn - version 0.11.1
- matplotlib - version 3.3.4
- scikit-learn - version 1.0.2
- statsmodels - version 0.13.2

## Acknowledgements
Give credit here.
- This project was inspired by Upgrad(IIITB) Linear-Regression-Case-Study-Bike-Sharing assignment.


## Contact
Created by [@yalagamsrinivas] - feel free to contact us!

