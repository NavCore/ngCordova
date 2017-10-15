# NgCordova: Angular 4 + Cordova boilerplate

This project is using Angular 4 + Cordova boilerplate configurated to work together so you can start building your great Hybrid Cordova Mobile Apps in Angular 4.

## Installation

* Install Node.js from: https://nodejs.org/en/download/
* Install Cordova using: `npm install -g cordova`
* Clone ngCordova repository: `git clone https://github.com/NavCore/ngCordova.git`
* Go to ngCordova repository: `cd ngCordova`
* Install dependencies: `npm install`

## Development server

* Development project folder is `src/`. You should start building your Angular 4 app there!
* Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Angular project base URL

* For Android App to work, change base url in index.html to: `<base href="file:///android_asset/www/">` or simple: `<base href=".">`
* For iOS App to work, change base url in index.html to: `<base href="./">` or `<base href=".">`
* Then build the Angular project

## Build Angular project

* Run `ng build` to build the Angular project. 
* The build artifacts will be stored in the `www/` directory. 
* Use the `-prod` flag for a production build.

## Adding Cordova platform

* Go to ngCordova repository: `cd ngCordova`
* List available Cordova platforms: `cordova platform ls`
* Add a desired platform: `cordova platform add [ browser | android | .. ]`

## Run Cordova app

* After adding Cordova platform, we can run our app in desired platform: `cordova run [ browser | android | .. ]`
* There is a known problem with emulating Android app using: `cordova emulate android`, so use `cordova run android`

## Build Cordova project

* Run `cordova build [ browser | android | .. ]` to build the Cordova project.
* For example android build .apk is located in: `platforms/android/build/outputs/apk/`
