---
layout: default
title: Welcome to Birb.JS!
nav_order: 1
---

# Welcome to Birb.JS!
Birb.JS is a Discord API wrapper for Node.JS. It's built to be simple, yet powerful. With just a few lines of code, you can get a Discord bot connected to the Discord API.

## Notice: In Development
**Birb.JS is still in development. It is highly recommended you don't use it until it's ready.** You can view the current progress of this project on GitHub: [BirbJS/Birb](https://github.com/BirbJS/Birb).

## Installation
Birb.JS is listed on [npm](https://www.npmjs.com/package/birb)! You can install it by running `npm install birb --save`.

### Optional Dependencies
- [erlpack](https://npmjs.com/package/erlpack) for faster serialization of websocket data: `npm install erlpack --save`
- [zlib-sync](https://npmjs.com/package/zlib-sync) for websocket compression: `npm install zlib-sync --save`

Most, if not all, of these dependencies require [node-gyp](https://github.com/nodejs/node-gyp), which some users may struggle to install (mostly due to very unhelpful errors). If you're on Windows and having issues, try running `npm install windows-build-tools --global`. If you're on Ubuntu, try `sudo apt install build-tools`. *Remember that these are optional dependencies. If you're struggling, feel free to ignore them. Birb.JS will only use them if they are available.*

## Example
Connect to the Discord API:
```js
const { Client, Intents } = require('birb');
let client = new Client({
    intents: new Intents(Intents.ALL),
});

client.listen('ready', () => {
    console.log('Connected to the Discord API!');
});

client.connect('your_token_here');
```
