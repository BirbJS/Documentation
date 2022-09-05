---
layout: default
title: Guild
parent: Classes
grand_parent: Reference
has_toc: false
nav_order: 1
---

[Birb](/) / Guild

# Class: Guild

## Hierarchy

- [`GuildPartial`](GuildPartial.md)

  ↳ **`Guild`**

## Table of contents

### Constructors

- [constructor](Guild.md#constructor)

### Properties

- [afkChannelId](Guild.md#afkchannelid)
- [afkTimeout](Guild.md#afktimeout)
- [approximateMemberCount](Guild.md#approximatemembercount)
- [approximatePresenceCount](Guild.md#approximatepresencecount)
- [available](Guild.md#available)
- [bannerHash](Guild.md#bannerhash)
- [boostCount](Guild.md#boostcount)
- [boostProgressBarEnabled](Guild.md#boostprogressbarenabled)
- [boostTier](Guild.md#boosttier)
- [client](Guild.md#client)
- [defaultMessageNotificationsLevel](Guild.md#defaultmessagenotificationslevel)
- [deleted](Guild.md#deleted)
- [description](Guild.md#description)
- [discoverySplashHash](Guild.md#discoverysplashhash)
- [explicitContentFilterLevel](Guild.md#explicitcontentfilterlevel)
- [features](Guild.md#features)
- [iconHash](Guild.md#iconhash)
- [id](Guild.md#id)
- [isOwner](Guild.md#isowner)
- [maxMembers](Guild.md#maxmembers)
- [maxPresences](Guild.md#maxpresences)
- [maxVideoChannelUsers](Guild.md#maxvideochannelusers)
- [members](Guild.md#members)
- [mfaLevel](Guild.md#mfalevel)
- [name](Guild.md#name)
- [nsfwLevel](Guild.md#nsfwlevel)
- [preferredLocale](Guild.md#preferredlocale)
- [publicUpdatesChannelId](Guild.md#publicupdateschannelid)
- [rulesChannelId](Guild.md#ruleschannelid)
- [splashHash](Guild.md#splashhash)
- [stickers](Guild.md#stickers)
- [systemChannelFlags](Guild.md#systemchannelflags)
- [systemChannelId](Guild.md#systemchannelid)
- [vanityUrlCode](Guild.md#vanityurlcode)
- [verificationLevel](Guild.md#verificationlevel)
- [welcomeScreen](Guild.md#welcomescreen)
- [widgetChannelId](Guild.md#widgetchannelid)
- [widgetEnabled](Guild.md#widgetenabled)

### Methods

- [edit](Guild.md#edit)
- [fetch](Guild.md#fetch)
- [isPartial](Guild.md#ispartial)

## Constructors

### constructor

• **new Guild**(`client`, `guild`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](Birb.md) |
| `guild` | [`APIGuild`](modules.md#apiguild) |

#### Overrides

[GuildPartial](GuildPartial.md).[constructor](GuildPartial.md#constructor)

#### Defined in

src/classes/Guild.ts:172

## Properties

### afkChannelId

• **afkChannelId**: ``null`` \| `string`

The channel ID (snowflake) of the guild's AFK channel as a string

#### Defined in

src/classes/Guild.ts:50

___

### afkTimeout

• **afkTimeout**: `number`

The guild's AFK timeout in seconds

#### Defined in

src/classes/Guild.ts:54

___

### approximateMemberCount

• **approximateMemberCount**: `undefined` \| `number`

An aproximation of the guild's member count (not exact)

#### Defined in

src/classes/Guild.ts:145

___

### approximatePresenceCount

• **approximatePresenceCount**: `undefined` \| `number`

An aproximation of the guild's user presence count (not exact)

#### Defined in

src/classes/Guild.ts:149

___

### available

• **available**: `boolean` = `false`

It is recommended to check if this value is `true` before performing actions
on the guild. If this value is `false`, the guild is unavailable due to a 
temporary Discord outage.

#### Inherited from

[GuildPartial](GuildPartial.md).[available](GuildPartial.md#available)

#### Defined in

src/classes/GuildPartial.ts:21

___

### bannerHash

• **bannerHash**: ``null`` \| `string`

The guild's channel list banner hash (not URL)

#### Defined in

src/classes/Guild.ts:121

___

### boostCount

• **boostCount**: `undefined` \| `number`

The amount of boosts the guild has

#### Defined in

src/classes/Guild.ts:129

___

### boostProgressBarEnabled

• **boostProgressBarEnabled**: `boolean`

Whether or not the guild has enabled the nitro boost progress bar

#### Defined in

src/classes/Guild.ts:165

___

### boostTier

• **boostTier**: [`GuildPremiumTierLevel`](GuildPremiumTierLevel.md)

The guild's boost level

#### Defined in

src/classes/Guild.ts:125

___

### client

• **client**: [`Birb`](Birb.md)

The Birb client

#### Inherited from

[GuildPartial](GuildPartial.md).[client](GuildPartial.md#client)

#### Defined in

src/classes/GuildPartial.ts:11

___

### defaultMessageNotificationsLevel

• **defaultMessageNotificationsLevel**: [`GuildMessageNotificationLevel`](GuildMessageNotificationLevel.md)

The default message notification level of the guild

#### Defined in

src/classes/Guild.ts:71

___

### deleted

• **deleted**: `boolean` = `false`

`true` if the guild is no longer available to the client (e.g. the client has
left or was kicked from the guild), `false` otherwise

#### Defined in

src/classes/Guild.ts:170

___

### description

• **description**: ``null`` \| `string`

The guild's description

#### Defined in

src/classes/Guild.ts:117

___

### discoverySplashHash

• **discoverySplashHash**: ``null`` \| `string`

The guild's discovery splash screen hash (not URL)

#### Defined in

src/classes/Guild.ts:42

___

### explicitContentFilterLevel

• **explicitContentFilterLevel**: [`GuildExplicitContentFilterLevel`](GuildExplicitContentFilterLevel.md)

The explicit content filter level of the guild

#### Defined in

src/classes/Guild.ts:76

___

### features

• **features**: [`GuildFeature`](modules.md#guildfeature)[]

The features enabled for the guild

#### Defined in

src/classes/Guild.ts:81

___

### iconHash

• **iconHash**: ``null`` \| `string`

The guild's icon hash (not URL)

#### Defined in

src/classes/Guild.ts:34

___

### id

• `Readonly` **id**: `string`

The guild's ID (snowflake) as a string

#### Inherited from

[GuildPartial](GuildPartial.md).[id](GuildPartial.md#id)

#### Defined in

src/classes/GuildPartial.ts:15

___

### isOwner

• **isOwner**: `boolean` = `false`

If `true`, the client's user is the guild's owner

#### Defined in

src/classes/Guild.ts:46

___

### maxMembers

• **maxMembers**: `undefined` \| `number`

The maximum amount of members the guild can have

#### Defined in

src/classes/Guild.ts:109

___

### maxPresences

• **maxPresences**: `undefined` \| ``null`` \| `number`

The maximum amount of presences the guild can have

#### Defined in

src/classes/Guild.ts:105

___

### maxVideoChannelUsers

• **maxVideoChannelUsers**: `undefined` \| `number`

The maximum amount of users allowed to watch a stream in the guild

#### Defined in

src/classes/Guild.ts:141

___

### members

• **members**: [`GuildMemberManager`](GuildMemberManager.md)

A manager that stores data on the guild's members

#### Defined in

src/classes/Guild.ts:101

___

### mfaLevel

• **mfaLevel**: [`GuildMFALevel`](GuildMFALevel.md)

The multi-factor authentication moderation requirement level of the guild

#### Defined in

src/classes/Guild.ts:85

___

### name

• **name**: `string`

The guild's name

#### Defined in

src/classes/Guild.ts:30

___

### nsfwLevel

• **nsfwLevel**: [`GuildNSFWLevel`](GuildNSFWLevel.md)

The explicit content level for the guild (set by Discord, mainly for iOS)

#### Defined in

src/classes/Guild.ts:157

___

### preferredLocale

• **preferredLocale**: `string`

The preferred locale of the guild (defaults to `en-US`)

#### Defined in

src/classes/Guild.ts:133

___

### publicUpdatesChannelId

• **publicUpdatesChannelId**: ``null`` \| `string`

The channel ID (snowflake) of the guild's updates as a string

#### Defined in

src/classes/Guild.ts:137

___

### rulesChannelId

• **rulesChannelId**: ``null`` \| `string`

The channel ID (snowflake) of the guild's rules channel as a string

#### Defined in

src/classes/Guild.ts:97

___

### splashHash

• **splashHash**: ``null`` \| `string`

The guild's invite splash screen hash (not URL)

#### Defined in

src/classes/Guild.ts:38

___

### stickers

• **stickers**: `undefined` \| `any`[]

A manager that stores data on the guild's stickers

#### Defined in

src/classes/Guild.ts:161

___

### systemChannelFlags

• **systemChannelFlags**: [`SystemChannelFlags`](SystemChannelFlags.md)

The flags that affect the guild's system messages (e.g. welcome messages)

#### Defined in

src/classes/Guild.ts:93

___

### systemChannelId

• **systemChannelId**: ``null`` \| `string`

The channel ID (snowflake) of the guild's system message channel as a string

#### Defined in

src/classes/Guild.ts:89

___

### vanityUrlCode

• **vanityUrlCode**: ``null`` \| `string`

If the guild has a vanity invite code, the guild's invite code

#### Defined in

src/classes/Guild.ts:113

___

### verificationLevel

• **verificationLevel**: [`GuildVerificationLevel`](GuildVerificationLevel.md)

The verification level of the guild

#### Defined in

src/classes/Guild.ts:67

___

### welcomeScreen

• **welcomeScreen**: `any`

The guild's Welcome Screen and Membership Gating settings

#### Defined in

src/classes/Guild.ts:153

___

### widgetChannelId

• **widgetChannelId**: `undefined` \| ``null`` \| `string`

If the guild has enabled the HTML widget, the channel ID (snowflake) of
the guild's widget channel as a string

#### Defined in

src/classes/Guild.ts:63

___

### widgetEnabled

• **widgetEnabled**: `undefined` \| `boolean`

`true` if the guild has enabled the HTML widget, `false` otherwise

#### Defined in

src/classes/Guild.ts:58

## Methods

### edit

▸ **edit**(`options`, `reason?`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`GuildEditOptions`](modules.md#guildeditoptions) |
| `reason?` | `string` |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Defined in

src/classes/Guild.ts:297

___

### fetch

▸ **fetch**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Inherited from

[GuildPartial](GuildPartial.md).[fetch](GuildPartial.md#fetch)

#### Defined in

src/classes/GuildPartial.ts:36

___

### isPartial

▸ **isPartial**(): `boolean`

#### Returns

`boolean`

`true` if this is a partial guild, `false` otherwise.

#### Overrides

[GuildPartial](GuildPartial.md).[isPartial](GuildPartial.md#ispartial)

#### Defined in

src/classes/Guild.ts:427
