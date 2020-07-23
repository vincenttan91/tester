# Project 2: Housing Price Prediction Model At Ames, Iowa, United States of America

### Problem Statement
Real Estate has always taken up a huge share of investment market around the world. However, most of the housing price are still benchmarked manually by experienced appraiser. Hence, it would really helpful to property investor if a predictive model can be created to find out any undervalued property listing and maximize their profit.

---

### Executive Summary
According to Forbes rich list in 2018, out of the 22 billionaires in Singapore, 16 of them are real-estate tycoons. The total fortune came up to a staggering $43.7 billion, which grew up to nearly 10 percent from the previous year [(Channel News Asia, 2018)](https://www.channelnewsasia.com/news/singapore/forbes-rich-list-tycoons-billionaires-2018-10564388). We cannot deny that all the successful real-estate investors have had either natural talent or decade-trained experience in them to tell a good or bad property listing or development project apart. Nevertheless, it would be fascinating if we could unravel and quantify the investors' - or ordinary home-buyer - judgement with the help of Data Science. So we set out a journey to create a machine learning model that could benchmark a property pricing based on its attributes.

In this project, we will develop a predictive model on housing sale price using regression technique. The model would be trained using an extensive training historical data and be evaluated with a testing set on its predictive performance. We believe that a model like this would be very valuable for any real state agent or home-buyer to set a benchmark pricing to judge whether a property listing is over or under-valued.

The dataset that we are using are part of housing sales record between 2006 and 2010 in Ames, Iowa from the Assessor’s Office. Originally contained 113 variables describing 3970 property sales, the data were used in calculation of home values for the city’s assessment process. It was then cleaned and refined by Dean de Cock from Truman State University, down to only 80 variables focusing on the quality and quantity of many physical attributes of the property [(Dean de Cock, 2011)](http://jse.amstat.org/v19n3/decock.pdf).

Due to the extensive number of attributes of more than 80, no data dictionary is given for the current project. For the full list, you may refer to [this link](https://github.com/vincenttan91/Ames_Housing_Prediction/blob/master/data_dictionary.txt).

---

### Conclusion/Recommendation
The predictive model that we have created is fairly accurate for houses that ought to priced at $350,000 and below - with error of up to ±50,000 for most cases. However, the accuracy falls short for houses above $350,000, constantly under-valueing the property price. This error might be caused by the limited number of training data with houses priced above this value. The model will be much improved if we could expand our training data with more property transaction record from Ames, especially with houses sold above $350,000.

Generally, our regression model is able to predict at a fairly good accuracy on both the training data and holdouts, with RMSE at $25,407 and $29,256 (from Kaggle). The RMSEs are higher than expected, given the average house value in Ames is only at $181,515. However, RMSE tends to exaggerate the error due to outliers, so for this case, we may also refer to the MAE of our training data, which is only at $18,160 (much better than the RMSE).
