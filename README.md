# Flipkart mobile price range prediction : Classification

![download](https://github.com/user-attachments/assets/fc518633-3e60-4a24-b8eb-fe1095557ff9)

# Project Summary -
One of the most popular and widely bought devices nowadays is the mobile. New mobile devices are released daily, often with updated software and more capabilities. Every day, tens of thousands of mobile phones are sold and bought. As a result, price estimate and prediction are crucial components of consumer strategy since a new product must be offered at the right price for customers to consider it suitable to purchase. People frequently make poor selections when buying mobile phones because they lack the tools needed to double-check the pricing. I created various categorization models utilising information about various mobile phone aspects in order to handle this problem.The developed model is then used to predict the price range of the new mobile phones.

The major goal of this research is to determine whether there is a correlation between a mobile phone's price range and its characteristics, which predicts whether the phone will be inexpensive(0), mid-range(1), expensive(2), or extremely expensive(3). To correctly categorise the data into appropriate price ranges, we will employ a variety of classification methods.

According to our dataset, there are 2000 records of mobile phone data with 21 characteristics that include category and numerical values. Fortunately, the dataset does not contain any null values and has a clear explanation of the features involved. After that, exploratory data analysis and data visualisation, i provided a brief explanation of the link between the characteristics and the label, or dependent variable, as well as a suggestion of which features to choose for the following step.

# Problem Statement
Companies seek to understand mobile phone sales statistics and the elements that influence prices in the cutthroat mobile phone industry.

The goal is to determine if there is any relationship between a mobile phone's features (such as RAM, internal memory, etc.) and its selling price. Instead of predicting the exact price in this scenario, we must provide a price range showing how high the price is.

# Variables Description
1. id : ID

2. battery_power: Total energy a battery can store in one time measured in mAh

3. blue: Has bluetooth or not

4. clock_speed: speed at which microprocessor executes instructions

5. dual_sim: Has dual sim support or not

6. fc: Front Camera mega pixels

7. four_g: Has 4G or not

8. int_memory: Internal Memory in Gigabytes

9. m_dep: Mobile Depth in cm

10. mobile_wt: Weight of mobile phone

11. n_cores: Number of cores of processor

12. pc: Primary Camera mega pixels

13. px_height: Pixel Resolution Height

14. px_width: Pixel Resolution Width

15. ram: Random Access Memory in Megabytes

16. sc_h: Screen Height of mobile in cm

17. sc_w: Screen Width of mobile in cm

18. talk_time: longest time that a single battery charge will last when you are on call

19. three_g: Has 3G or not

20. touch_screen: Has touch screen or not

21. wifi: Has wifi or not

# Conclusion

![download](https://github.com/user-attachments/assets/4413e8cf-a423-4971-bff5-38825ec445e8)

1.Due to their capacity to resist the effects of the dataset's lowest performing features, tree-based models (XGBoost and Random Forest in our example) perform by far the best. Cross validation and hyperparameter adjustment greatly improve the performance of the Random Forest Classifier and XGBoost.

2.Based on our core goal, which is to forecast the price range for mobile devices. Out of all the models used, including Naive Bayes, Knn, Random Forest, XGBoost, and SVM, Logistic Regression had the greatest performance.

3.For each price range, a similar type of distribution can be seen when analysing the distribution of numerical characteristics with regard to the taget variable, although there are still certain standout features. When we take into account that characteristics like "talk_time," "sc_h," "sc_w," "clock_speed," "fc," "int_memory," "m_dep," "mobile_wt," "n_cores," and "pc" are not linearly connected to price range, for example, we see a distribution that is comparable.Additionally, each feature, whether it increases in value or decreases in value in relation to the price, will influence the projected pricing of mobile devices.

4.The least effective model for our dataset is the Knn model.

5.Except for a few elements like the front camera, pixel resolution height, and screen width, the most of the numerical features had a consistent distribution.

6.With the exception of the characteristic "three_g,"   most of the categorical features shared a similar distribution or count. There were hardly any entries for mobile devices that don't support 3G.

![Screenshot (19)](https://github.com/user-attachments/assets/9e085270-d47e-4e28-9395-a7d9f36b50cf)

