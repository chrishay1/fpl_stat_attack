# FPL Stat attack
### What is this?
This github repository contains code to scrape data from the Fantasy Premier League website, and present that data via an R Shiny app.

The R Shiny app is currently hosted at;

<html>https://chrishay1.shinyapps.io/FPL_stats/</html>

The app contains a couple of different widgets, one to help identify recent player form, and another to rank teams based on upcoming 
fixture difficulty.

### Fantasy premier league
The Fantasy Premier League is a game run by the English Premier League. Players in this game select footballers playing in the real
English Premier League. The league can be accessed via the below website;

<html> http://fantasy.premierleague.com </html>

This website provides some statistics on player performance, but only to a limited degree. The purpose of this code is allow players
to 
1. apply additional filters to the data that are not available via the main website (particularly for recent statistics)
2. see what teams have good upcoming fixtures based on the fixture difficulty ranking (as per the main website).

There are currently 3 main files within this repository; others have been included to demonstrate some of my working.

### Main files.
1. UI.R
2. Server.R 
These two files are the basis of the Shiny application. 
3. update_fpl_data.R
This file scrapes the data from the FPL website into an easily read CSV file, that is then saved to Dropbox. This is done as scraping the 
FPL data can be time consuming. 
