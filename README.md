## This is cont.. 
from the hashlips minting dapp.  Assuming you have completed all the steps to this point and have a completed build folder.  Some changes need to be done in order to host your app on heroku.  

## -- Hosting your dapp using heroku. --

 1.  Edit the gitignore to include the build folder.
 2.  Create a NODEjs server file
 3.  Edit the package.json file
 4.  Create a Git account.
 5.  Create a Heroku account. 


## Set package.json file to now host your app using node:


set Line 24.    "start": "node server".


##  Edit /server.js to run on your local machine.


set Line 11.   app.listen(3000);



##  Edit /server.js to run on heroku: 


set Line 11.   app.listen(process.env.PORT);


## The build file needs to be included by deleting it from the gitignore file Section 50


 delete build/


 ## Git and Heroku commands


 git push orgin master

 git push heroku master