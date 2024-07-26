# StockPortal
My implementation real time stock fetching and rendering of the data was based on c# desktop application (this was full working application as i got license from
activ financial sdk at that time and i was able to work time series data, option chain data, screen level 1 data) And to some extent i was also involved in stock order execution development 

I was not able to implement the web based solution at that time (2014-15)  because there was no proper web socket implementation was availbe.And apart from that the problem in activ financial sdk if user with different rights  logged in and later on if some logged in with different rights then previous logged in user's right would be overwritten with rights of later logged in user ( i.e if some one logged in with rights of fetch only US exchanges based stock  data  and later on if some other user logged in with rights of fetching  stock data of global wide exhnages then previous user rights will be overwritten with rights of later users andvice versa).

Due to such kind of hurdles, company management was reluctant to implement web based solution because it was going to be catastrophy (user credentials were 
verified by central gateway not from end-user applications, so there was 99% chances above mentioned scenario was going to happen frequently).   

With rise of websocket and push  based architectures, it is possible to implement web solutions. Following is list of vendors that are currently providing 
real time stock data 
1. Alpha Vantage
2. Finnhub
3. IEX Cloud
4. Polygon.io
5. Alpaca

So far i am only  able to  explore two of above mentioned vendors (Finnub and alpaca) and  i am only implement solution for Finnhub because most of  time alpaca's free 
data providing service is remaining online 

I have implemented soluton based on #reactjs, #nodejs, #javascript  

Note : This project is only  for academic purposes. Because i have compared with yahoo's financial data and it feels like finnhub free real time stock data 
is delayed data ( i have compared compared trade volume and price parameters
