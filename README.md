# PWA-Text-Editor

## Description

When using a text editor, whether its online or offline, it is important that your data is stored and is displayed when you return to the page. When this app crossed my table, it did not have functionalty to store and display user entered data. Additionally it was not a Progressive Web App (PWA) as it has no webpack bundle, service worker, or manifest. I have modernized this app so that it meets all of the basic PWA criteria. You can even download the app from your broswer and use it offline!

## Installation

To use this app you can simply access this link: https://quiet-thicket-94927.herokuapp.com/

If by any chance you wish to deploy this app locally, begin by downloading this repo onto your local machine. Follow the next steps:

- Install all dependencies with the `npm i` command on the repo root level
- Launch the app using `npm run start`
- Head over to http://localhost:3000/ and try it out

## Usage

When you have accessed the app using one of the methods above, you will be presented ith the text editor. You can enter or alter any data that you like. When you click off of the text editor area, your changes will be saved instantly. Behind the scenes I am utilizing the IndexedDB to store your data. If you close the page and access the url again, you will notice that your text remains just as you left it. This is also thanks to the IndexedDB!

If you lose internet connect, have no worries. I implemented a service worker that immediately caches the necessary resources to run the app. This means you do not need an internet connection to run the app after you have accesed it.

This app can also downloaded to your machine from the browser. To do so, click the save icon to the left of the url bar in your broswer window. You will notice that any text that you have entered is also acessible on the downloaded app.

Enjoy!

![Screenshot of Text Editor](./assets/img/Text%20Editor%20Screenshot.png)
