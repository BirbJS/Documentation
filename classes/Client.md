---
layout: default
title: Client
nav_order: 2
parent: Classes
---

# Client
The Client class is the main entry point for Birb.JS. It is used by the end user to connect to Discord, receive events, and send some commands to the Discord API.

## Properties
| name                   | description           | type                             | optional | default     |
|:-----------------------|:----------------------|:---------------------------------|:---------|:------------|
| options                | The client options    | Object                           | false    |             |
| options.intents        | Intents to use        | [Intents](/classes/Intents)      | false    |             |
