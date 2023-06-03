---
title: Tank Controller Manager Instructions
---
## Components of the Web App

### The Main Screen

![Tank Controller Manager Interface](/assets/images/TCM_front_page.png)

The default page of the TCM is the tank controller interface, modeled to look as close to the physical controller as possible for ease of use.
This interface shows the same information as the physical controller's display, and allows all of the same inputs as the physical controller. It follows the same instructions as listed on the device software page of the Tank Controller [here](/docs/15-device-software/).

The three tabs at the bottom, Keypad, Information, and Files, can be used to switch between the three pages of the web app.

At the top left of the screen is the menu which allows tanks to be added or removed from the list, as well as switching between the currently displayed tank.

![Tank Controller Manager Menu](/assets/images/TCM_menu.png)

### The Information Page

![Tank Controller Manager Information Page](/assets/images/TCM_information.png)

The second page of the TCM is the information page, an example of which is shown above with blank values.
This page lists important information about the currently selected tank controller.

In addition to this, the page offers two more features.
The fields marked with pencils allow direct edits to be made, bypassing the interface of the main page.
Clicking on the field will bring up a popup, which will allow a new value to be entered and sent to the controller.

The button just above the information tab, labeled upload file for arbitrary path, will bring up a standard file upload interface that allows .txt and .csv files of 10 KB or less to be uploaded directly to the tank controller's memory.

### The Files Page

This page will allow the viewing and download of files such as controller logs stored on the tank controller.