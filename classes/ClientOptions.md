---
layout: default
title: ClientOptions
parent: Classes
has_toc: true
---

# ClientOptions
The ClientOptions class stores the options for the client. It is used by the [Client](/classes/Client) class. You do not need to create an instance of this class, as it is created for you when creating the [Client](/classes/Client).

### Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Constructor
{: .d-inline-block }

PRIVATE
{: .label .label-red }

`new ClientOptions(options)`

| name                   | description           | type                             | optional | default     |
|:-----------------------|:----------------------|:---------------------------------|:---------|:------------|
| options                | The client options    | Object                           | false    | none        |
| options.intents        | Intents to use        | [Intents](/classes/Intents)      | false    | none        |
| options.cdnDomain      | The Discord CDN domain | String                          | true     | cdn.discord.com |
| options.inviteDomain   | The Discord invite domain | String                       | true     | discord.gg |
| options.gatewayDomain  | The Discord gateway domain | String                      | true     | gateway.discord.gg |
| options.gatewayVersion | The Discord gateway version | Number                     | true     | 9 |

# Properties

## intents
The intents to use when connecting to Discord.

**Type:** [Intents](/classes/Intents)

## cdnDomain
The Discord CDN domain.

**Type:** String
**Default:** `cdn.discord.com`

## inviteDomain
The Discord invite domain.

**Type:** String
**Default:** `discord.gg`

## gatewayDomain
The Discord API gateway domain.

**Type:** String
**Default:** `gateway.discord.gg`

## gatewayVersion
The gateway version to use when communicating with Discord.

**Type:** Number
**Default:** `9`

# Methods

## get(key)
Gets a value from the options.

| name                        | description                           | type                    |
|:----------------------------|:--------------------------------------|:------------------------|
| key                         | The key to get                        | String                  |

**Returns:** Any

## set(key, value)
Sets a value.

| name                        | description                           | type                    |
|:----------------------------|:--------------------------------------|:------------------------|
| key                         | The key to set                        | String                  |
| value                       | The value to set it to                | Any                     |

**Returns:** [ClientOptions](#constructor)

## remove(key)
Removes a value from the options.

| name                        | description                           | type                    |
|:----------------------------|:--------------------------------------|:------------------------|
| key                         | The key to remove                     | String                  |

**Returns:** [ClientOptions](#constructor)

## has(key)
Check if the options contains a key.

| name                        | description                           | type                    |
|:----------------------------|:--------------------------------------|:------------------------|
| key                         | The key to check fo                   | String                  |

**Returns:** Boolean

## clear()
Removes all values from the options.

**Returns:** [ClientOptions](#constructor)

## toDefault()
Sets all values to their defaults.

**Returns:** [ClientOptions](#constructor)
