---
title: Google Docs Integration
---

The Tank Controller devices can report current pH and Temperature readings for the tank to a Google Sheet.  
This will allow viewing of the current tank status from anywhere you have an internet connection.
Google Docs integration, however, is optional and the basic functionality of the device is not affected if you do not complete these steps.

## Creation of the Google Sheet and Script
To perform the following steps you will need a Google account, and be signed into that account.
Go to the following link to find the Tank Controller Monitor template: [Monitor Template](https://docs.google.com/spreadsheets/d/1IrcRgtypfAYEB23MBk3Bh1gWOA9KFftv4Z9MHpWA5ns/edit?usp=sharing)

Make a copy of this template for yourself by clicking on "File" in the menu, then "Make a copy".
This will bring up the "Copy document" dialog box.
In the box labeled "Name", the default name will be "Copy of Tank Controller Monitor Template". Instead, give the document any name that you wish. Then click "OK".

Next find the spreadsheet ID of your copy of the Tank Controller Monitor spreadsheet and copy it.  You can find it in the URL address of the sheet. I have an example below in which the spreadsheet ID is marked in red.

https://docs.google.com/spreadsheets/d/<span style="color:red">17csF55yQlx2HJP9xseCQdg8_DI6Znge3YeeOjI1ZSZs</span>/edit#gid=0

Navigate to the url: script.google.com.
Click the "New project" button in the upper left of the page to start a new script.  
This will bring you to a code window.  
Into the code window paste this code: [Google Script Template](https://docs.google.com/document/d/1oyupNPuR41Uw8On4gPO-X4F8IePKwD16_Qx1jdiEuqA/edit?usp=sharing).

Then replace the section that says "\<enter spreadsheet ID here\>" with your spreadsheet ID.

Next, in upper right click the "Deploy" button, then "new deployment".  In the window that pops up, click the cog next to "Select type", then select "Web app".  Then under "Configuration", type in anything that makes sense under "Description". Under "Execute as" select "Me". Then under "Who has access", select "Anyone" (not "Anyone with Google account"). Then click "Deploy".
![Google script deployment](/assets/images/google_script_deploy.png)

When you click "Deploy", another window will appear that says "The Web App requires you to authorize access to your data.".
Click "Authorize access" and select your Google account in the next window.
Next a window will say "Google hasn't verified this app".
Click "Advanced" in the lower left and corner and "Go to Untitled project (unsafe)".
In the next window click "Allow".
Another window will show up that will say "Deployment successfully updated.".
Under that it will say "Web app", and under that "URL."  
Copy that URL by clicking the "Copy" button below it and save it somewhere you can find it again such as in a text document or a Word document.
You will need this URL when setting up PushingBox in the next section of the instructions.  
![Google script deployment](/assets/images/Google_script_URL.png)

Now, lets test if the script is working. Paste the URL you just saved with "?tankid=1&tempData=23&pHdata=4.555" added to the end of it into a new browser tab.
Does "ok" show up in the browser?
If so, check your Tank Controller Monitor spreadsheet.  
You should see the data show up under "Raw_Data" tab that report Tank 1 with a temperature of 23 and a pH of 4.555. The data should also appear for Tank 1 under the Dashboard tab.

## Setting up PushingBox
Navigate to https://www.pushingbox.com/ and click "Login with Google" in the upper right hand corner. Complete the login with your Google login credentials

Next, click on "My Services" in the menu towards the top of the page, then click the "Add a Service" button on the next page.
Now click on "Select this service" next to "Custom URL".  It will be at or near the bottom of the options.
Give this service a name in the top box labeled "Name of your CustomURL configuration:".  It doesn't really matter what the name is, as long as you can recognize it.
Now, paste google script macro "Current web app URL" into "Root URL" (without the "?tankid=1&tempData=23&pHdata=4.555" you added for testing).
Leave method as GET and click the "Submit" button.
Now click on "My Scenarios", then in the box under "Create a scenario or add a device" put in some name of your choosing (I use "Tank ID, Temp and pH Push"), and click "Add".
Now, click the "Add an Action" button.  Then, click "Add and action to this service" next to the service you made in the previous step.
In the box under "Data" copy and paste in the text: "?tankid=$tankid$&tempData=$tempData$&pHdata=$pHdata$" (without the quotes). The click "Submit".
Now, copy DeviceID that should be right under the scenario name. It should start with "v".
Now, copy that DeviceID into Tank Controller Arduino code on line 7 where it says PushingBoxIdentifier. You must have the quotes around the DeviceID.
