# ML_Model_Dataset
Creating a machine learning model and training the dataset.

In my ambition to learn more about AI and ML related concepts, I made a small write up related to obtaining a dataset, defining/training a model, and applying statistical methodology and ML fundamentals in hopes of learning more about the subject. See below.

[Abstract]

(Made-up business case) - We work at a mid-sized firm that provides frozen products at stores or grocery stores. One product in particular is a lunch plate containing portions of avocadoes. Due to the high cost of avocadoes (indeed with respect to the cost of the other ingredients contained in the plate), the business has requested for a predictive analytics model to be applied to the ongoing cost of the ingredient to ensure product profitability is kept. (Ex: Changing the tolerance of the mix of ingredients present while retaining the appropriate mix of ingredients as expected by the Brand based on present market need and sale value at the store). 

[Creating and Obtaining the Dataset]

For this we will need to obtain a dataset of the avocadoes purchased over time, along with the sale value.

[CSV]

The above CSV was obtained from Kaggle [here](https://www.kaggle.com/datasets/neuromusic/avocado-prices). (..and as mentioned, is entirely unrelated to the made-up business case)

[Creating the dataset]

With the list provided to us, this should be as simple as applying some statistical models and retrieving the running average and perhaps near-market time volatility by the end of the day! (I'll be home by 5!) 

Unfortunately we first need to acquire or assume the dataset, understand or interpret it manually, and then prepare or clean it up so it may be used as an appropriate model. Great, that doesn't sound too bad! :)

[Assessing the Data]

Without going too in depth, the data was provided with a description of the columns. This includes fields like Date, AveragePrice (average price of 1 avocado), Total Volume (total number of avocados sold), and other fields like Small Bags (# of avocadoes sold in a bunch, or bag).

Some of these fields sound strange or unecessary. I also don't know how accurate the data is. Were the counts made at the store or by shorthand at the market? It's possible that the results are estimated (in which case we would want to accomodate for such 'innacuracy' of the source data within our model somewhere).

Let's import the dataset with Jupyterlabs utilizing pandas and review it.
![image](https://user-images.githubusercontent.com/9099847/235455615-de26b4d0-19b1-49c3-9408-101fdb88bd47.png)

Alright. We are now able to read in the data. Based on best practices we know we should cleanup unecessary data to reduce clutter or confusion when building a model for our dataset. Let's clean up the data. 

1. Get a quick count of columns, filesize, etc.


3. Second, remove junk data. Drop columns if they are irrelevant.


5. Merge or combine columns if or where it makes sense.


7. Clean up data types, currency, fractions, dates, etc. In our case we have decimals for whole unit counts. Let's format it to whole number avocadoes.


9. Take a second look for final validation of our dataset, and save the updated or cleaned up version to our drive.

Let's look again at our completed dataset. Looking a lot better!


[Train the model]





[1.5]: https://raw.githubusercontent.com/Ignitetechnologies/Windows-Privilege-Escalation/main/linked.png

# Follow us on [![alt text][1.1]][1] [![alt text][1.3]][1.4] [![alt text][1.5]][1.6]

![image](https://github.com/Ignitetechnologies/Vulnhub-CTF-Writeups/blob/master/vulnhub.png?raw=true)

