# Automated NodeJS Push Messages Notifier.

This is a simply demostration using both GCM and Web Notification API, this is an automated process where registration ids are sent in real time using
socket.io.

## Setup :

In order to get the dependecies make sure to do the following : 

```terminal
# npm install
```

This command will download and install all needed dependecies.

## Application Configuration : 

1. Head to [Google cloud Console](console.cloud.google.com) and create new application.
2. In Google APIs area, enable the GCM API.
3. By now you will have an **app_id** and **app_secret** keep those ids in a secure location.
4. Now in our project files, go to the **manifest.json** file and update the **gcm_sender_id** with the one retreved from you project.
5. Now go to the **server.js** file and do the following :

 ```js
      const sender = new gcm.Sender('<put app_secret here>');
       ```

By now the project is fully configured and everything is set to launch.

## Run the Application : 

In order to run the application go to your command line of choice and add the following commad :

```terminal
# npm start
```

Now to to **localhost:3000** approuve the notification **permission** and by now you will see the notification promt in your desktop.


Happy Coding :)

Peace !

