# Speedy Cheers Architecture Design:

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

 
 ## User App Features :

### Technical : 
 - SPA
 - User login
 - Profile creation
 - Integration of Google Map API’s
 - Option to select the number of SpeedyCheeers
 - Enter/Select the activity, Payment integration

### Functional : 
 - User needs to inform SpeedyCheers on the activity/select from a list of activities from the app.
 - User will have option to select  the number of speedy cheers.
 - User has the option to choose the time
 - Upon arrival both party authenticates via top sent
 - Once the task is completed the user cancels the service and price is received by the user from SpedeyCheer calclateSpeedyCheerPrice() function.

### User App Functionalities :

 - Sends the current GPS location of user along with user unique key/identifier to a Centralised (zone specific) data centre.
 - Refresh in 10 secs to get the updated location and store in DB
 - High Availability, high throughput, low latency
