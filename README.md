 # Speedy Cheers Architecture Design:

![Diagram](Speedy Cheers System Design)
 
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


 
 ## SpeedyCheers Features :

 ### Technical:
 - SPA 
 - Cheer login
 - Profile creation
 - Integration of Google Map API’s
 - Option to view the order placed via user

 ### Functional: 
 - Nearest cheer gets notified when a user request a SpeedyCheer
 - While accepting a booking a Speedy Cheer(s needs to know what activity user is requesting and accept/reject
 - If rejected it should be notified to the user and restart the process
 - Once accepted ETA is sent to the user
 - Upon Arrival user and Speedy cheer authenticates via OTP and triggers calclateSpeedyCheerPrice()function
 - Amount gets calculated for each SpeedyCheer  with base price $10 and incremented in every 5 minutes 
 - Once user stops the service via User app the total amount calculated from above function is sent to user for  payment
