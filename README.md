This is my 'Python for everybody' capstone project. 
As a hobby Fantasy Football player, I was interested in automation of data gathering and filtering processes.

Data collected from: Understat.com (free football statistics site with advanced metrics for 6 european soccer leagues).

Python libraries used: understat, pandas, matplotlib, seaborn, asyncio, json, aiohttp, sqlalchemy, adjustTexts.

I used the data from current EPL season. I took a look at what players have biggest differents between goals scored and xG (expected goals metric). 
In order to do that, I loaded data from Understat.com with understat library, made a json file out of output, 
converted it to pandas dataframe, added some columns and converted it to sql table. 

After that I used pandas, matplotlib and seaborn for visualisation purposes.
In order to be more fair to the players with less minutes played, I created xG_diff/90 column, 
which represents difference between xG value and goals scored in terms of 90 minutes (one full football match).

And finally I wanted to make something beautiful, so I chose 'key_passes' and 'shots' columns to make the scatter plot of best 20/21 EPL players. 
That took me a while because of the overlapping points :) I fixed it with adjustTexts library.

In order to do all this, I worked my way through all py4e specialization, 
3-4 Kaggle free micro courses to obtain basic knowledge about most popular and useful python libraries and tons of googling, 
mainly through extremely helpful Stackoverflow site.
