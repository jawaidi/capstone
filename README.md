Modeling time to fill freight loads


I scraped freight load data from dat.com.  It is a website where shippers post about a million loads each day and truckers bid on the loads.  My goal was to predict the time that it takes to fill a load after a shipper posts the load.  I expected to find features in the load data that would let me predict the fill time.  However once I began scraping the data, I found very limited features and the features did not seem to have any effect on the fill time.  The features were origin, destination, weight, shipper and the time the shippers posted the load.  I was left to model the fill time against the load time.


I used a linear regression model which did not explain the variance of the data because the fill time depends on other factors not captured in my model and were not easily available such as traffic conditions, fleet and driver availability.


One challenge that I faced while scraping included the fact that shippers would repost a load when it was not filled making it difficult to capture the original load time as a predictor.