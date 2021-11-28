---
layout: default
title: Client
parent: Classes
has_toc: true
---

# Client
The Client class is the main entry point for Birb.JS. It is used by the end user to connect to Discord, receive events, and send some commands to the Discord API.

### Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Constructor
`new Client(options)`

| name                   | description           | type                             | optional | default     |
|:-----------------------|:----------------------|:---------------------------------|:---------|:------------|
| options                | The client options    | Object                           | false    | none        |
| options.intents        | Intents to use        | [Intents](/classes/Intents)      | false    | none        |

# Properties

## token
The token to use to connect to Discord. **Never share your token!**

**Type:** String

## options
The options used to initialize the client.

**Type:** [ClientOptions](/classes/ClientOptions)

# Examples
Create a basic client that listens to all intents:
```js
const { Client, Intents } = require('birb');
const client = new Client({
    intents: new Intents(Intents.FLAGS.ALL)
});
client.connect("token")
```
Just listen to guild and guild message events:
```js
const { Client, Intents } = require('birb');
const client = new Client({
    intents: new Intents(Intents.FLAGS.GUILDS, Intents.FLAGS.GUILD_MESSAGES)
});
client.connect("token")
```
