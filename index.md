# Welcome to Birb.JS!
Birb.JS is a Discord API wrapper for Node.JS. It's built to be simple, yet powerful. With just a few lines of code, you can get a Discord bot connected to the Discord API.

## Example
```js
const { Client, Intents } = require('birb');
let client = new Client({
    intents: new Intents(Intents.ALL),
});

client.on('ready', () => {
    console.log('Connected to the Discord API!');
});

client.connect('your_token_here');
```
