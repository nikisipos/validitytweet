# Validity labs tweets

Analysis of tweets and the reactions to it from Validity Labs.

## Usage
The 'twint_download' file downloads the twitter data from the twitter account of validity labs into an sqlite database ('twint_validitylabs_wo_retweets.sqlite').

'analyse' makes the analysis and generates .png plots.

## Results
There are 2 different appoaches in the analysis, one checks the frequencies of words appearing in the most and least popular tweets based on likes. The other checks how the reactions to the tweets changed with time.

### Wordcounts 
'analyse' extracts the words from the least/most popular tweets (10% most and least popular) and how often they appear. It deletes all words that appear in both groups as they won't make a difference in the number of likes. Finally it produces a wordcloud from the words that remain.  

### Time evolutionc and histogram
'analyse' takes the monthly sums of likes and shows on a plot how they changed since the beginning of the tweets. It also produces a histogram that shows how many different types of reactions there are.

## Further improvements
A similar wordcount analysis with hashtags would probably be really informative. Also it should be checked what could cause the sudden increase in likes since April 2017, see plot (eg. check number of followers, cryptocurrency changes etc.). Also the distribution of likes could be checked based on part of the day/day of the week(it could be more likely that people read posts during the day and not the night etc.) read posts during the day and not the night etc. The retweets and the actual people reacting should also be checked. 

## Technical information
The code is written in Python 3 and 'pip3-install' contains the necessary modules.


