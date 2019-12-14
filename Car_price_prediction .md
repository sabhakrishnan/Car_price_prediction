# Car_price_prediction
Non-Linear Model
This is a car sales data set which is taken from Analytixlabs. This is a continuous data set which include several predictors.From this data set we have to predict car sales by using machine learning Techniques.
So lets work on this dataset together and carry out which machine learning technique is best suited for prediction.
I am using Python language you can use any language for this .So go for it and enjoy.
If you have any query related data you can freely post your query

# Features of Datasets
'Manufacturer', 'Model', 'Type', 'Min.Price', 'Price', 'Max.Price',
       'MPG.city', 'MPG.highway', 'AirBags', 'DriveTrain', 'Cylinders',
       'EngineSize', 'Horsepower', 'RPM', 'Rev.per.mile', 'Man.trans.avail',
       'Fuel.tank.capacity', 'Passengers', 'Length', 'Wheelbase', 'Width',
       'Turn.circle', 'Rear.seat.room', 'Luggage.room', 'Weight', 'Origin',
       'Make'
       
# Data Cleaning:
       ->The Data cleaning includes Exploration of the data as well as, transformation of the data for the usefull analysis.
       ->Here the price of the car is the problem statement.
       ->So, the bi-variate analysis made for analysing the features which is making significant difference in the car price.
       ->Which is shown in EDA.
       ->Price Vs Origin: says that the cars price are recorded as both inside and outside of USA.
       ->Price Vs Cylinders : It says the variation in the price according to the number of cylinders. But using boxplot we can say that there are significant different in the each cylinder for the price prediction. so, we can include this feature for predicting our column.
       ->Price Vs Airbags: Since different catagories in the airbag feature making  the significant difference in the price, so it is also taken into consideration for making the analysis.
       ->Here, the 'Man.Trans.Avai' feature has the string column as 'Yes' and 'No'. Here the 'Yes' says that avalability of manual transmission 'No' says that automatic transmission. So, this particular feature is label encoded as 0 and 1, wheer 0 as manula transmission and 1 as automatic transmission.
       ->The 'airbag' column has 3 different catagories as 'Airbags for Drivers and Passengers', 'Airbags for Drivers only' and 'None'. These 3 catagories are created as dummay variable columns in the data set for further analysis. 
       ->The 'Drive Train' column has the 3 catagories as 'Front' as front wheel drive, 'Rear' as rear wheel drive and '4WD' says that 4 wheel drive', so these feature is also created dummies for including in to the analysis. 
       ->The 'Cylinders' feature are created with dummies for the model building.
       ->After, creating the dummies, we can drop the original columns before building the model. 
       ->These detaied steps are followed in the Exploratory data analysis.
    
# Model Building
    The Target variable is Price, so its an contineous variable. So we need to use the Linear Regression model to predict the price.
    I used the MVLR model using K-Fold technique and got the bias and varience error of the model.
    Then i have tried with the polynomial regression for the 2 features according to the domain knowledge. 
    I have tried using PCA for the better accuracy of the model.
    After PCA my model performed well for the prediction of price.
    Then i tried bagging and boosting but it doenst make any changes in the Base PCA Regression model.
    So, my PCA MVLR model is the better mode for prediction of car-Price
    
       
