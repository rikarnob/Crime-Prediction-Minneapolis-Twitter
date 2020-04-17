# TrendsMarketplace-Team15

Team Members - Patrick Hoban, Sam Musch, Rikarnob Bhattacharya, Sarah Wang, Mohammed Saad Ahmad, Yuwen Yan

Repository for all codes we used for the Fall Trends Marketplace Project. This repository contains code that was used to access Twitter API, merge it with crimes, poverty and weather data as well as code used for training the XgBoost model (used for time series prediction).

The repository also contains the PPT we used for the voicethread, the flyer we used for the Marketplace event and the dashboard that was on display.

The idea of the project was to be able to predict crime using factors outside of previous incidents. The avenue we set out to explore was the predictive power of tweets from a region, weather information and demographic make-up of the same region, in predicting crime.

Tweets, being textual in nature, have the potential of indicating the general sentiment prevailing in a region in addition to providing information about the latest goings-on. The idea behind incorporating each element was - 

> Tweets - we gathered tweets from local news agencies to get a sense of the happenings; we considered a lagged value of the sentiment (e.g. for predicting crime on day T, we used tweets from day (T-1)) to predict crimes since sentiment of a day prior is more likely to have an impact on events of the following day

> Weather - it is common knowledge that people tend to go out more when it's sunny outside. And crimes take place more when there are more people outside. But is that a blanket statement we can make? 

(E.g. we found burglary/theft shoots up when there is more than 3-4 inches of snow!)

> Demographic - indicator of how well-off a region within a city is which can be used as an excellent indicator for crime. Less well-off neighborhoods would tend to have a higher crime rate


* 1. PreppingData.ipynb - Twitter API data and merging with crimes and weather data
* 2. XGBoost.ipynb - Merging dataset from 1s output with topic distribution and poverty data
* 3. Crime Dashboard.twb - Tableau dashboard containing visuals for our descriptive analysis as well as the time-lapse on the crime counts throughout 2019
* 4. Flyer_Team 15_Predicting Crime in Minneapolis.pdf - Takeaway hand-out distributed at the booth on final presentation day
* 5. Marketing Poster.pdf - Marketing poster setup at 3 spots as standalone advertising terminals. The content was created based on learnings from Lee Thomas's session on 'Elevator Pitches'
* 5. Trends Final Presentation_Use Cases for booth.pptx - These use cases and insights were showcased on a pull-out display board, to demonstrate the real-life application of the analysis and solution. This includes visualizations made in both Tableau as well as Amazon Quicksight
