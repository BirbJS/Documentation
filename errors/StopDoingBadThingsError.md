---
layout: default
title: StopDoingBadThingsError
parent: Errors & Warnings
has_toc: true
---

# StopDoingBadThingsError
The StopDoingBadThingsError error is an error you'll see if you try and do something you *really* shouldn't.

## StopDoingBadThingsError: self-bots (non-bot automated accounts) are banned from accessing the Discord API Gateway by Discord and are not supported by the Birb.JS library
You tried to use Birb.JS to create a self-bot. As Discord puts it:

> Discord's API provides a separate type of user account dedicated to automation, called a bot account. Bot accounts can be created through the applications page, and are authenticated using a token (rather than a username and password). Unlike the normal OAuth2 flow, bot accounts have full access to all API routes without using bearer tokens, and can connect to the Real Time Gateway. **Automating normal user accounts (generally called "self-bots") outside of the OAuth2/bot API is forbidden, and can result in an account termination if found.**

We've deliberately made sure that, if Birb.JS is told your account is not a bot, that it will immediately throw an error, terminate (not close) your connection to Discord, and exit the process. If you're looking to use Birb.JS to create a self-bot, you'll need to find a different library.

```
StopDoingBadThingsError: self-bots (non-bot automated accounts) are banned from accessing the Discord API Gateway by Discord and are not supported by the Birb.JS library; to use Birb.JS you must use a bot account otherwise you may have your account BANNED by Discord; use a bot token instead
```
