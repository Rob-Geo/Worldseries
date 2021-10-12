# Can Machine Learning Predict Who Will Win The World Series?

*This project is still being modified. The proposed completion date is December 12, 2019*

In October 2019, the Houston Astros and the Washington Nationals made it into the World Series. It was the Astro's 3rd World Series and first since winning back in 2017, and the National's first ever World Series appearance. Thanks to a combination of hometown pride (Go ‘Stros!) and a desire to merge current events with current learning, a group of students decided to use machine learning to predict the World Series. 

### Data Collection and Cleanup

The primary data source for this project is [baseball-reference.com]( https://www.baseball-reference.com). 

Steps:
* Download CSVs that covered fielding, pitching and hitting statistics by team for the season
* Download outcomes of all games played by each team
* Join these together into one dataframe and drop any columns that wouldn’t add any significant value to our analysis


### The Machine Learning Model

This project utilizes the Random Forest Classifier

Different criteria was applied to several models to see which would yield the most accurate prediction. 
* Astros vs. Nationals
* Division winners
* All teams (this is the criteria we chose for our model)
* All teams with only selected features 

All predictions ranged between .57 -.61 in accuracy 

### Twitter Sentiment Analysis

The sentiment analysis aims to pull live tweets during each game in an attempt to understand fans attitude and feelings towards each team as well as pinpoint specific phenomenon impacting fan’s world series experience. 

* Using Twitter’s Api, a call was sent every 15 minutes to gather fans tweets about each team (@Astros, @Nationals, @WorldSeries). 
* VADER, a trained AI, evaluates each tweet, giving it an overall “compound score” expressing whether the tweet was positive, negative or neutral in nature.

### Technologies Used
* Python and Pandas - Used for data collection and cleanup
* sklearn - Used for machine learning model
* VADER - Used for Twitter sentiment analysis


### Authors
* [Rob Edwards](https://github.com/Rob-Geo)
* [Kristin Lucas](https://github.com/klucas11)
* [Marc Thomas](https://github.com/MarcThomas-Mo)
* [Valeria Bejarano](https://github.com/vbejarano)
