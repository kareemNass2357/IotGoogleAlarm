# IotGoogleAlarm
Alarm system , works with google assistant , with wifi arduino or ESP 


#Process Overview
when the user starts the alarm by saying “ turn seucity system on “

google sends to a webhook that changes one of the virtual pins, the system  turns on , 

when a movement does occurs  , a virtual pin gets changed that sets off a webhook in the blyink , 

the webhook starts an event that the alarm has been set off , as well as notify the user 

if the user tries and fails to open the alarm , a wrongPass event is set off , and the user is notified

when the user enters the right password by saying “turn security off, the password is “ 

a google assistant will trigger a webhook that sends the password for checking in the esp and turns the system off


#IFTT Instructions
| Tables        | Are           |
| ------------- |:-------------:|
| col 3 is      |  
 	When the alarm is turned on , if a movement happens, it changes a virtual pin , that in the blynk app , triggers a web hook, the web hook sents a message to the user warning him  	
|
| col 2 is      |  

 	When the system receives a password from a virtual pin , if the password is incorrect, it sends the user a message warning him , throught a webhook that starts from blynk , and sends a message to the user	
     |
| zebra stripes |  
 

 


 

 







	The user sends a password with the google assistant , and sends the password to a webhook that changes a virtual pin directly and the esp catches it and tries to compare it io its own password 

| zebra stripes | When the user tells google assist to trunt he system on , it changes a virtual pin through a webhook directly and the esp , turns the alarm on , and notifies the user with the screen 	
     |
| zebra stripes | are neat      |     |



#Web hook instructions