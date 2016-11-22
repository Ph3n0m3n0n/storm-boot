Welcome to Storm-(boot), a lightweight, minimal framework with built-in user management and authentication using Node.js, Express and Stormpath. Please be sure to follow the setup instructions below. this application will not run without proper setup first. It will throw an error.

SETUP:
Before this app can be used, you have to set up a few things. 

1. Go to https://api.stormpath.com/register and setup an account.

2. Login to your account and click on `Manage API Keys` on the right-hand side under the Developer Tools box.

3. On the menu bar at the top of the screen, click on the option that says `Applications`, then the big blue button on the right that says `Create Application`.

4. Name the application and provide a description. You can leave the other options at their default settings. Click `Create`.

5. Once you create the application, it will appear in the list under the Applications tab. Select it from the list. 

6. Next go to the `Accounts` tab in the left menu bar and select your directory. Copy the `HREF` link at the top of the page. You will need it for later.

7. Scroll to the bottom of the page and find the `API Keys` dropdown menu. Click the big blue button that says "Create API Key". An API key will automatically be downloaded to your local system. 

8. Find the downloaded file. It should end in `'.properties'. Open this file up in a text editor. Here are your API Key ID and secret.

9. It is a best practice to store confidential information in environment variables (don’t hard-code it into your application). You should store your confidential Stormpath information in environment variables. You can do this by running the following commands in the shell:

 `export STORMPATH_CLIENT_APIKEY_ID=YOUR_ID_HERE
  export STORMPATH_CLIENT_APIKEY_SECRET=YOUR_SECRET_HERE
  export STORMPATH_APPLICATION_HREF=YOUR_APP_HREF`

FOR WINDOWS USERS, USE THESE COMMANDS INSTEAD: 

 `set STORMPATH_CLIENT_APIKEY_ID=YOUR_ID_HERE
  set STORMPATH_CLIENT_APIKEY_SECRET=YOUR_SECRET_HERE
  set STORMPATH_APPLICATION_HREF=YOUR_APP_HREF` 

  ** Checkout https://docs.stormpath.com/nodejs/express/latest/configuration.html for full configuration documentation.


Now that you have setup your app with Stormpath, you can start using it! Check out your authentication. 

Login screen: `localhost:3000/login`
Register screen: `localhost:3000/register
Forgot password screen: `localhost:3000/forgot`

After a user registers and logs in, you have access to this information through your admin page on the Stormpath website! Now you can store and collect data from your users without ever having to connect a database. Have fun!


