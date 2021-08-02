# A 'Progressive' budget tracker (PWA practice)
The 'budget-tracker is a basic Progressive Web Application (https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps) that allows a user to track travel expenses and income whilst online and offline. 

The budget tracker uses service-worker functionality combined with IndexedDB alloiwing for offline storage. 

This application was undertaken as an educational program to learn approaches to developing PWAs. The majority of the front-end came pre-built, so my own work on this application is associated with back-end functionality, initiating and implementing service-worker functionality, interactions with IndexedDB and syncing between IndexedDB and MongoDB during offline-online state changes.  

A working demo of the application can be viewed at:
https://budget-tracker-mongo-practice.herokuapp.com/

## Author
github.com/daniel-gregg

## Description
This budget-tracking application was developed as an initial foray into learning about the creation of PWA applications using service workers, IndexedDB, Dexie (npm) MongoDB and mongoose (npm).

Key learnings from this project were:
- Setting up service worker functionality
- Setting up IndexedDB to receive post/get/put requests when offline and to update when online
- Using offline/online states to manage database syncing

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)

## Installation
- You must have Node installed on your computer. See here https://nodejs.org/en/download/. 
- Check that you have the latest version of npm installed. In node type this into the console: 'npm install npm@latest -g'
- npm must first be initialised using 'npm init' in your working directory
- dependencies can then be installed using 'npm install PACKAGE' where 'PACKAGE' refers to the relevant dependency. 

### Dependencies include:
- mongoose
- express
- dotenv
- morgan
- dexie
- workbox + workbox-config

Additional option dependies are:
- nodemon

### Set up your local environment
- You will need to point the local server host to your own local mongoDB. First create a new DB in your mongo console or through your bash/cmd console. 
- Alternatively you can set up a Heroku mongoDB and set up your environmental variables following the outlines posted on Heroku (namely get your connection string and replace the '<password>' and 'yourDB' sections with the respective values).

## Usage
The application is designed as a single-user app. The user can add new transactions and view the transaction history as well as their current remaining budget.

## Screenshots
Home screen:
![homescreen view](/assets/homescreen.png?raw=true "Homescreen view")





