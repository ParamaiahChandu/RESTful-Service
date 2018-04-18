# RESTful-Service
Implementing RESTful Service with the given data  
  
I have developed a RESTful web service that hosts weather information. I have added end points to my application to accept input data as input parameters to do GET and POST operations. This will return JSON result in plain text format to the user.  
  
The root API for this web service is 'http://18.219.111.32/'. When user enters this in his browser, he is going to get a welcome message in JSON format as shown in the screen shot '1 Start Page.PNG'.  
  
If the user enters end point as 'http://18.219.111.32/historical/', list of the dates for which the weather infromation is available will be displayed in hos browser in JSON format as shown in the screen shots. The starting and ending of this JSON output looks like the '2 Historical starting.PNG' and '2 Historical Ending.PNG' screen shots.  
  
If the user enters end point as 'http://18.219.111.32//historical/YYYYMMDD/', weather information for that particular date is displayed in JSON format as shown in the screen shot '3 Historical Particular Date.PNG'. If there is no record with the date entered, 404 error occurs.  
  
For POST and DELETE, we need 'Postman' google extension.  
  
If user want to POST, the end point to enter is 'http://18.219.111.32/historical/' in the Postman extension. Here user need to keep the option as POST and have to select 'raw' in the body section. In the responce, format should be JSON. User must enter data In JSON format as shown in the screen shot '4 Post Adding.PNG'. The result can be validated by selectin GET option and using the end point of date POSTed as shown in the screen shot '4 Post Result.PNG'.  
  
Delete is similar to POST but instead of POST, user need to select DELETE. The end point is 'http://18.219.111.32/YYYYMMDD'. When user clicks send in the Postman after entering proper endpoint, a success message will be displayed as shown in '5 Delete Date.PNG'. The deletion can be verified either in browser or Postman. The user cannot see the deleted date as shown in '5 After Delete in Chrome.PNG' and '5 After Delete in Postman.PNG'.  
  
Inaddition to these, forcast is done. The end point for forecast is 'http://18.219.111.32/Forecast/YYYYMMDD'. User can see 7 days in forecast as shown in '6 Forecast.PNG'.  
