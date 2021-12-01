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

- TOC
{:toc}

# Constructor
`new Client(options)`

| name                   | description           | type                             | optional | default     |
|:-----------------------|:----------------------|:---------------------------------|:---------|:------------|
| options                | The client options    | Object                           | false    | none        |
| options.intents        | Intents to use        | [Intents](/classes/Intents)      | false    | none        |
| options.debug          | Debug mode            | Boolean                          | true     | false       |

```js
const { Client, Intents } = require('birb.js');
const Client = new Client({
  intents: new Intents(Intents.FLAGS.ALL)
});
```

# Properties

## token
The token to use to connect to Discord. **Never share your token!**

**Type:** String

## options
The options used to initialize the client.

**Type:** [ClientOptions](/classes/ClientOptions)

# Methods

## listen(event, listener)
{: .d-inline-block }

EVENT LISTENER
{: .label .label-purple }

Registers a listener for the specified event.

| name                        | description                           | type                    | optional       |
|:----------------------------|:--------------------------------------|:------------------------|:---------------|
| event                       | The event to listen to                | String                  | false          |
| listener                    | The function to be ran when emitted   | Function                | false          |

```js
client.listen('message', message => {
    if (message.content === 'hi') {
        message.reply('hello!');
    }
});
```

**Returns:** void

## unbind(event)
Unbinds a listener that was previously bound using the [`listen`](#listeneventlistener) method to the specified event.

| name                        | description                           | type                    | optional       |
|:----------------------------|:--------------------------------------|:------------------------|:---------------|
| event                       | The event to unbind                   | String                  | false          |

```js
client.unbind('message');
```

**Returns:** void

## emit(event, ...args)
{: .d-inline-block }

EVENT EMITTER
{: .label .label-purple }

Emits an event that can be detected using the [`listen`](#listeneventlistener) method on the specified event.

| name                        | description                           | type                    | optional       |
|:----------------------------|:--------------------------------------|:------------------------|:---------------|
| event                       | The event to unbind                   | String                  | false          |
| ...args                     | One or more arguments to pass         | any                     | true           |

```js
client.emit('customEvent', 'something happened!');
```

**Returns:** void

## connect(token)
Connects to Discord using the specified token. **Never share your token!**

| name                        | description                           | type                    | optional       |
|:----------------------------|:--------------------------------------|:------------------------|:---------------|
| token                       | Your bot's token                      | String                  | false          |

```js
client.connect('your_token_here');
```

**Returns:** void

## debug(...message)
{: .d-inline-block }

INTERNAL
{: .label .label-yellow }

Emit a debug message. Printed to console if debug mode is enabled.

| name                        | description                           | type                    | optional       |
|:----------------------------|:--------------------------------------|:------------------------|:---------------|
| ...message                  | The message to emit                   | any                     | false          |

**Returns:** void

## warn(...message)
{: .d-inline-block }

INTERNAL
{: .label .label-yellow }

Emit a warning message. Printed to console if debug mode is enabled.

| name                        | description                           | type                    | optional       |
|:----------------------------|:--------------------------------------|:------------------------|:---------------|
| ...message                  | The message to emit                   | any                     | false          |

**Returns:** void

# Examples
Send `hello!` when a member says `hi`:
```js
const { Client, Intents } = require('birb');
const client = new Client({
    intents: new Intents(Intents.FLAGS.ALL)
});

client.listen('message', (message) => {
    if (message.content === 'hi') {
        message.reply('hello!');
    }
});

client.connect("token")
```
