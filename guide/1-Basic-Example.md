---
layout: default
title: Basic Example
parent: Guide
has_children: false
has_toc: false
nav_order: 1
---

[Birb](/) / [Guide](/guide) / Basic Example

# Creating a Basic Bot

This bot will:

    - Connect to the Discord real-time gateway
    - Listen for the `ready` event (which is fired once the client is fully ready)
    - Listen for the `guild created` event (which is fired when the client joins a server)

## Example

### TypeScript

```ts
import { Birb, Guild } from 'birb';

const client = new Birb({
    intents: ['GUILDS'],
});

client.when('ready', () => {
    console.log('Connected to Discord!');
})

client.when('guild created').do((guild: Guild) => {
    console.log(`I just joined ${guild.name}!`);
});

client.setToken(process.env.DISCORD_TOKEN!);
client.fly();
```

### JavaScript

```ts
const { Birb } = require('birb');

const client = new Birb({
    intents: ['GUILDS'],
});

client.when('ready', () => {
    console.log('Connected to Discord!');
})

client.when('guild created').do((guild) => {
    console.log(`I just joined ${guild.name}!`);
});

client.setToken(process.env.DISCORD_TOKEN);
client.fly();
```
