# Polymer2-server-reload-build-Ecmascript-5


### Technical data
This application use: the Polymer server for build, compile and bundled in  **es5-bundled** and **es6-bundled**
 and BrowserSync for loading any change. **With old browsers (ej. IE11) isn't possible read Ecmascript 6 code, with this compiler is possible make a website for these browser and same time minify all files (javascript and html)**.
I changed the root for links for adapt the reload. 

##### Original app
https://github.com/Polymer/shop


### Setup

##### Prerequisites


Install [polymer-cli](https://github.com/Polymer/polymer-cli):

    npm install -g polymer-cli

Install [bower.json]:

    bower install -g 

Install [NPM - package.json]:

    npm install -g 



##### Setup

    # download the zip file or
    git clone https://github.com/vitantonioc/Polymer2-server-reload-build-Ecmascript-5.git
    cd Polymer2-server-reload-build-Ecmascript-5
    npm install -g polymer-cli
    npm install
    bower install

### Start the development server

    npm run start

### Build ecmascript 5 and ecmascript 6 (bundled and unbundled)

    npm run dev
    
    After this command open "build" folder and copy the files for use

### Build

Build presets provide an easy way to define common build configurations in your `polymer.json` file. There are 2 build presets we put in `polymer.json` file in Shop:

**es5-bundled**

- js: {minify: true, compile: true}
- css: {minify: true}
- html: {minify: true}
- bundle: true
- addServiceWorker: true
- addPushManifest: true
- insertPrefetchLinks: true

**es6-unbundled**

- js: {minify: true, compile: false}
- css: {minify: true}
- html: {minify: true}
- bundle: false
- addServiceWorker: true
- addPushManifest: true
- insertPrefetchLinks: true

