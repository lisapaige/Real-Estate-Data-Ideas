# Real-Estate-Data-Ideas
An attempt to organize an on going brainstorm of ideas regarding real estate analytics

Big data tools for accessing state and local markets.  
Statistics and trends country(worldwide?) with subset capability in to state, city/county, zip codes, neighborhoods, etc.

## Graph Theory Ideas

### Identify and expand services for potential/existing clients
**Star**. 
Define r user levels X: x1 = Interstate, concurrent project investers, ... xr = First time buyer
For each level there is an ideal star K(1,n) where client is the central node, and n services are available to client level r. 
- nodes (order = n+1) represent client + services avaialbe to clients at level r
- edges (size = m) represent services being utilized; m between 0: potential client, to n: utilizing all n services available at level r
**Complete**. 
For potential recommender use: removing the client from the star and using complete graphs K(n) as the ideal
Train recommender on high size graphs and the progression to high size graphs 
LevelClass:
- input client attributes
- output client level r, with ideal star K(1,n)

### Identify and predict potential investment clusters
Spatial cluster analysis of trend plus first and second derivative trends
- mortgage attributes(increasing rate, higher LTV, deferral status, late payments, foreclosure)
- market features (pricing, list-to-close ration, days-on-market, broker remarks*)


## Regression Ideas
Filter data to desired market, train data on client level. 
### Model mean trends to see related features and get a feel for the market 
Note: confidence intervals will not include prediction variance.  
### Prediction for quantified decision making
Note: allow clients to dial in their risk tolerance based on changing prediction intervals
- purchase price 
- investment cost
- holding cost (genralized linear models (NB/Geom/Poisson for days-to-flip and days-on-market)
- closing cost/profession cost (agent, attorney, cpa) 

## Fun and Powerful Ideas
*Broker Remarks (ways to quantify these results coming...)*
Brokers are in the trenches and very much like to borrow language to use in their comments. Analyzing changes in Broker Remarks shouldn't be overlooked.  
### Can you tell which is Pre-Covid and which is Post_Covid?
![Denver 80207 Broker Remarks]()
