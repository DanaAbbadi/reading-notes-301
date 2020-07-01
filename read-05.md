# Getting Started on Heroku with Node.js

## Heroku

Heroku is cloud service platform for deploying applications to the web/cloud. It marks a good middle step between deploying a page on say Wordpress, and creating your own server. What deploying means is that the program and its data is on a server connected to the cloud, which is really just a big bunch of servers. When a page is deployed on Wordpress is put into the their servers, effectively out of your hands. You can control the page it self, the client side, but everything on the server-side is not for you to mess with. Of course if you build/buy your own server and set it up in a closet or your basement you have complete control of the server programming and settings. This requires more money and more expertise.


## Create an app via the command line

  * Step 1: Create repo on github
  
  * Step 2: Clone repo to local machine
   
           $ git clone [link from github]
  
  * Step 3: Create heroku app command:
  
           $ heroku create [app-name]
   
   Step 4: Deploy code
  
          $ git push heroku master
  
  * Step 5: Open the deployed app to see if it deployed correctly
  
         $ heroku open


## View Activity logs via the command line

    $ heroku logs --tail

## Locally run your app

    $ heroku local web

## Push local changes

    $ git add .
    $ git commit -m"Message"
    $ git push heroku master
    $ heroku open [app name] (open the app to check if changes went through)