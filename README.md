
<p align="center">
<img src="Images/santa.png" alt="Santa Cartoon Drawing" width="200" style="float: right; margin-right: 10px;"/>
</p>

Secret Santa App
============================================================================================================================================

Overview
--------

Do you want to add that personal touch to virtual Secret Santa? How about creating own app for people to take part!

Based off the guide here: [Build a Secret Santa App in 20 Minutes or less with PowerApps - April Dunnam - SharePoint Siren](https://www.sharepointsiren.com/2017/12/build-a-secret-santa-app-in-20-minutes-or-less-with-powerapps/)

Uses an Excel Table as the main Data Source

The App
-------

Huge shout out to April Dunnam's guide above as it acted as the starting point for creating this app, especially the random logic for the draw!

The App has 3 main sections

**Registration**

- Auto population of the fields is done by using "User()" function in PowerApp, I had no idea PowerApp was smart enough to pull this info before starting work on this: <https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/functions/function-user>

- Then the tick button is selected the inputs from the form at wrote into the Excel Table

- TODO: Check to see if the user is already registered so they can't register twice
- TODO: Hide address information & who has who from the spreadsheet so the values are hidden until displayed in the app? 

**Reveal / Draw**

- Using the Random Logic in the Blog post above will draw someone to buy a gift for

    o TODO: You can potentially draw yourself and this is why the re-draw button is included so room to improve the logic used here

- If you have already drew someone to buy for the next time you select this page you will be reminded who you are buying for rather than going back in to draw someone else

**Participants**

- Shows a list of everyone who has registered to take part so far

How to Import
-------
- Sign in to your PowerApp Environment > Apps > Import Canvas App > Upload the zip included in the repo > Import 

- Once App is Imported Edit go to: Data > Add Data > Connectors > Excel > OneDrive > Select SecretSanta2021_Template.xlsx included in this repo > Select Table 1 > Connect > Insert Auto Generated ID > Create


<p align="center">
  <img src="Images/elves.jpg" alt="Dancing Elves" width="700" />
</p>
