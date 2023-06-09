# ML_LinearRegression
Creating a machine learning model and training the dataset.
### Work in progress - May.05.2023
In my ambition to learn more about AI and ML related concepts, I made a small write up related to obtaining a dataset, defining/training a model, and applying statistical methodology and ML fundamentals in hopes of learning more about the subject. See below. 

## [Abstract]

(Made-up business case) - We work at a mid-sized firm that provides frozen products at stores or grocery stores. One product in particular is a lunch plate containing portions of avocadoes. Due to the high cost of avocadoes (indeed with respect to the cost of the other ingredients contained in the plate), the business has requested for a predictive analytics model to be applied to the ongoing cost of the ingredient to ensure product profitability is kept. (Ex: Changing the tolerance of the mix of ingredients present while retaining the appropriate mix of ingredients as expected by the Brand based on present market need and sale value at the store). 

## [Creating and Obtaining the Dataset]

For this we will need to obtain a dataset of the avocadoes purchased over time, along with the sale value.

### [CSV]

The above CSV was obtained from Kaggle [here](https://www.kaggle.com/datasets/neuromusic/avocado-prices). (..and as mentioned, is entirely unrelated to the made-up business case)

### [Creating the dataset]

With the list provided to us, this should be as simple as applying some statistical models and retrieving the running average or perhaps near-market time volatility by the end of the day! **(I'll be home by 5!)**

Unfortunately we first need to acquire or assume the dataset, understand or interpret it manually, and then prepare or clean it up in some way so it may be used as an appropriate model. **Great, that doesn't sound too bad! :)**

### [Assessing the Data]

>Without going too in depth, the data was provided with a description of the columns. This includes fields like Date, AveragePrice (average price of 1 avocado), Total Volume (total number of avocados sold), and other fields like Small Bags (# of avocadoes sold in a bunch, or bag).

Some of these fields sound strange or unecessary. I also don't know how accurate the data is. Were the counts made at the store or by shorthand at the market? It's possible that the results are estimated (in which case we would want to accomodate for such 'innacuracy' of the source data within our model somewhere). At this point we would also check with our business team for additional parameters such as a confusion matrix to be utilized prior to the data being cleaned up (it may make some columns more relevant!)

Let's import the dataset with Jupyterlabs utilizing pandas and review it.
![image](https://user-images.githubusercontent.com/9099847/235455615-de26b4d0-19b1-49c3-9408-101fdb88bd47.png)

Alright. We are now able to read in the data. Based on best practices we know we should cleanup unecessary data to reduce clutter or confusion when building a model for our dataset. Let's clean up the data. 

>1. Get a quick count of columns, filesize, etc.


>2. Second, remove junk data. Drop columns if they are irrelevant.


>3. Merge or combine columns if or where it makes sense.


>4. Clean up data types, currency, fractions, dates, etc. In our case we have decimals for whole unit counts. Let's format it to whole number avocadoes.


>5. Take a second look for final validation of our dataset, and save the updated or cleaned up version to our drive.

Let's look again at our completed dataset. Looking a lot better! :) 


## [Training the model]

For our model, we will utilize a linear regression model. Let's check our textbook again and make sure we have the basics correct.

![image](https://user-images.githubusercontent.com/9099847/235462815-9be67d54-d2da-468f-8282-3c1ce7d11c66.png)

# Setting the test

# Running the model

## [Retrieving the results]

At this point we're finished with our effort. The results were obtained and additional steps can be taken accordingly.

## [Deployment and Monitoring of our Model]

With the results provided, we can send this to our Ops team to create an automated pipeline to assist us or other analysts in reviewing the predictive model. This is covered in a separate repository located [here](https://github.com/endlessparadigm/ML_Model_Deploy). Let's remember to send the correct requirements so they know exactly what to do. 

## [Additional Analysis]

Additional strategies can now be taken to improve on our effort.
1. Return to the data source and verify with the author or data gathering authority on the accuracy or authenticity of the records. If the data was gathered from manual surveys, do we know the degree of error on it? Do we feel comfortable in regards to the quality of data entry or data entry validation in regards to the values kept.
2. Based on the model utilized, can we improve upon the existing model for more accurate results?
3. Similar to the points above, can we revise the specifications expected by the business or review the business parameters provided? How is this being translated to the manufacturing team?
4. 







https://www.sciencedirect.com/topics/mathematics/simple-regression-model#:~:text=The%20simple%20regression%20model%20assumes,term%20%CE%B5%20encompassing%20omitted%20factors.

```
> Y=a+bX+u

Where:

Y = Dependent variable(the variable that you are trying to predict )
X = Independent variable(the variable that you are using to predict Y )
a = the intercept
b = the slope
u = the regression residual.
```



