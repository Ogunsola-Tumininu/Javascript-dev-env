# Building a JavaScript developmnet environment
## Pridavanie editorconfig (vsteky file budu mat podobny styl)
## bit.ly/jsdevpackagejson
### node security project nsp (skontroluje node_modules) Prikaz je: nsp check [No known vulnerabilities found]
### set up Express (web server)

### vytvorenie webservera cez localtunnel
* Localtunnel: 1. Najpr spustit localhost: node buildScripts/srcServer. reserved.js        
* Localtunnel: 2. A potom sputit localhost: lt --port 3000 --subdomain branislav


```
 "scripts": {
    "prestart": "node buildScripts/startMessage.js",
    "start": "npm-run-all --parallel security-check open:src",
    "open:src": "node buildScripts/srcServer.js",
    "security-check": "nsp check",
    "localtunnel": "lt --port 3000 --subdomain branislav",
    "share": "npm-run-all --parallel open:src localtunnel"
  },
```


### Babel
zmena var experess = require('express') na import express from 'express'
a pridanie const


###Webpack: spoji vsetky assets do jedneho suboru
* bit.ly/2dSZwea
* pridanie webpacku do srcServer.js


