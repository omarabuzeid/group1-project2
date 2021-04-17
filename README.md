### Thomas & Omar's Project: The Musk Effect

## Challenge:
With the rise of social media, we have seen the simultaneous rise of prominent market influencers. The notion of a market influencer isn’t new. Prior generations were enraptured by star investors like Bill Miller, Peter Lynch and Warren Buffett. Today’s influencers however, aren’t defined by track record or expertise per say. The rapper Snoop Dogg, for example, was credited with sending the price of cryptocurrency dogecoin soaring after he tweeted an altered version of one of his album covers, showing himself with a “doge" head.

No market influencer is perhaps more infamous than Tesla CEO Elon Musk.  One January afternoon, Tesla Inc. Chief Executive Elon Musk sent out an 11-character tweet: “Gamestonk!!". The market reaction was perhaps unprecedented. Musk's followers sprung into action, and GameStop Corp. shares surged more than 150% overnight. The next day, analysts threw up their hands. Nothing apart from Mr. Musk’s tweet—which included a link to Reddit’s WallStreetBets forum—could explain why the stock soared.

Tesla meanwhile, Musk's very own company, has seen tremendous growth over the past 5 years.  With that said it is still a pretty volatile stock. Therefore, we decided to find out the effect Elon Musk's tweets on the price of Tesla's stock, and if so, whether or not a net positive trading strategy could be created to capitalize on said effects. 


## Model:
After preparing the necessary data to analyse sentiment within Mr. Musk's tweets, as well as retreiving the relevant stock market data, we began to work on our model. 
Our original plan for creating the model was to simply run random forrest on the existing data, while possibly messing with the different available data a little in order to produce better correlations between the sentiment analysis and the actual change in stock price. We encountered a few problems with this method, especially when it came to processing the data in a way that random forrest can understand. 
Eventually, we were able to process the data into an acceptable format, and from that cleaned data, random forrest was able to produce a high correlation with a low MSE value, indicating that the model was consistent in it's predicitons. 
Rather than only trying to predict the change in Tesla stock price, we also simplified to model to only predict the direction in which the stock price moved. This method produced better results, as we could use positive and negative sentiment to predict positive or negative stock change, a much simpler method. 

## Conclusions:
Ultimately, we were not able to produce a model that was able to beat our benchmark, which was simply the average change in price over the entirety of the dataframe. If we had more time, it's possible we would change the timeframe to only include TESLA's meteoric rise in the past few years, as there were 7 or so years with relatively little change. 
