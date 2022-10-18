# WeRateDogs Twitter Data Analysis and Visualization
## by Alvens Akinkunmi


## Introduction
>In this data wrangling project, I will first collect 3 different datasets that are related to WeRateDogs Twitter data. Then I will assess the data via both visual and programming assessment, and clean the data.
After the data gathering stage, data accessing stage, data cleaning stage and storing stage of the WeRateDog Twitter data,I continued to analysis and visualize the cleaned data. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. This analysis is based on a master WeRateDogs dataset that has been assessed and cleaned by me. I mainly used matplotlib module for my analysis, and it covered one-variable distribution.

### Gathering Data
>The first dataset is The WeRateDogs Twitter archive, i imported a csv file called 'twitter-archive-enhanced.csv'. I downloaded the  get tweet image predictions data provided in udacity classroom since i could twitter didn't grant me access to their API. The last dataset I gathered was additional data from Twitter API. I extracted the tweet_id, favorite_count and retweet_count from the third dataset.

### Assessing Data
>Firstly,I asssesed these data visually, both injupyter notebook and in Excel, and then programming assessment to find out the following data quality and tidiness issues.

#### Quality
##### Enhanced Twitter Archive:
> - Tweet_id column dtype is integer.
2. Timestamp column dtype is not in datetime.
3. There are 78 replies to be remoed from the dataset.
4. There are 181 retweets to be removed from the dataset.
5. Not every tweet has identified dog stages.
6. Wrong ratings i.e. the numerator and denominator ratings were given in different columns
7. Capitalize first letters in name column
8. Identify rating_denominator which is less than 10 and change to 10

##### Image Table
> - Tweet_id column dtype is int.
2. More than one predictions in for dogs in one single tweet.
3. There are non-dog predictions.

##### Twitter Extra Data
> - Wrong id column name
2. Count columns have object type instead of integer type.
3. Wrong id dtype format, integer instead of string

##### All three tables
> - Img_num is in wrong format, integer instead of string

#### Tidiness
##### Enhanced Twitter Archive
> - Dog stages are not in one column.
2. There are 2 columns (numerator and denominator) related to rating, should be combined

##### All three tables
> - The three tables are not merged

### Cleaning Data
>I used the basic Define-Code-Test methodology to clean all datssets. After cleaning the datasets, I merged the three datasets into a master dataset and saved it as twitter_archive_master.csv.
After saving the datasets into twitter_archive_master.csv, the dataset will be analysed and insights will be derived from various visuals that will be plotted.

## Insights
> I grouped all dogs in the data by name. It was gathered that most of the dogs are called by either the name, `A` which has the highest frequency of occurence, or by `Lucy`, which has the second highest frequency  and then by the name, `Charlie`.
The top rated breed as showned in the figure below is the `Dumber` with an average rating of `14`.
From the figure below, it could be seen that the least rated breed of dog from the WeRateDogs dataset is the `Japanese spaniel` with an average rating of `5`.
And lastly, the `Labrador retriever` was discovered to have the highest retweet count with a value of `79515`.
## Conclusion and Improvement
>From the visualizations, we can clearly state that people rated the Labrador retriever by retweeting, though, reasons for this couldn't be arrived at with the provided data.
There are more to explore with this data. For example, the stage of the dogs clearly has a lot missing. I haven't got a chance to explore the prediction model provided, and also there are other data i haven't analysed.


```python

```
