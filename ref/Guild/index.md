---
layout: default
title: "Guild"
has_children: true
has_toc: false
nav_order: 1
---

[birb](../README.md) / [Exports](../modules.md) / Guild

# Class: Guild

## Hierarchy

- [`GuildPartial`](../GuildPartial/index.md)

  ↳ **`Guild`**

## Table of contents

### Constructors

- [constructor](index.md#constructor)

### Properties

- [afkChannelId](index.md#afkchannelid)
- [afkTimeout](index.md#afktimeout)
- [approximateMemberCount](index.md#approximatemembercount)
- [approximatePresenceCount](index.md#approximatepresencecount)
- [available](index.md#available)
- [bannerHash](index.md#bannerhash)
- [client](index.md#client)
- [defaultMessageNotificationsLevel](index.md#defaultmessagenotificationslevel)
- [deleted](index.md#deleted)
- [description](index.md#description)
- [discoverySplashHash](index.md#discoverysplashhash)
- [explicitContentFilterLevel](index.md#explicitcontentfilterlevel)
- [features](index.md#features)
- [iconHash](index.md#iconhash)
- [id](index.md#id)
- [isOwner](index.md#isowner)
- [maxMembers](index.md#maxmembers)
- [maxPresences](index.md#maxpresences)
- [maxVideoChannelUsers](index.md#maxvideochannelusers)
- [members](index.md#members)
- [mfaLevel](index.md#mfalevel)
- [name](index.md#name)
- [nsfwLevel](index.md#nsfwlevel)
- [preferredLocale](index.md#preferredlocale)
- [premiumProgressBarEnabled](index.md#premiumprogressbarenabled)
- [premiumSubscriptionCount](index.md#premiumsubscriptioncount)
- [premiumTier](index.md#premiumtier)
- [publicUpdatesChannelId](index.md#publicupdateschannelid)
- [rulesChannelId](index.md#ruleschannelid)
- [splashHash](index.md#splashhash)
- [stickers](index.md#stickers)
- [systemChannelFlags](index.md#systemchannelflags)
- [systemChannelId](index.md#systemchannelid)
- [vanityUrlCode](index.md#vanityurlcode)
- [verificationLevel](index.md#verificationlevel)
- [welcomeScreen](index.md#welcomescreen)
- [widgetChannelId](index.md#widgetchannelid)
- [widgetEnabled](index.md#widgetenabled)

### Methods

- [edit](index.md#edit)
- [fetch](index.md#fetch)
- [isPartial](index.md#ispartial)

## Constructors

### constructor

• **new Guild**(`client`, `guild`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `client` | [`Birb`](../Birb/index.md) |
| `guild` | [`APIGuild`](../modules.md#apiguild) |

#### Overrides

[GuildPartial](../GuildPartial/index.md).[constructor](../GuildPartial/index.md#constructor)

#### Defined in

src/classes/Guild.ts:66

## Properties

### afkChannelId

• **afkChannelId**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:32

___

### afkTimeout

• **afkTimeout**: `number`

#### Defined in

src/classes/Guild.ts:33

___

### approximateMemberCount

• **approximateMemberCount**: `undefined` \| `number`

#### Defined in

src/classes/Guild.ts:57

___

### approximatePresenceCount

• **approximatePresenceCount**: `undefined` \| `number`

#### Defined in

src/classes/Guild.ts:58

___

### available

• **available**: `boolean` = `true`

#### Overrides

[GuildPartial](../GuildPartial/index.md).[available](../GuildPartial/index.md#available)

#### Defined in

src/classes/Guild.ts:63

___

### bannerHash

• **bannerHash**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:51

___

### client

• **client**: [`Birb`](../Birb/index.md)

#### Inherited from

[GuildPartial](../GuildPartial/index.md).[client](../GuildPartial/index.md#client)

#### Defined in

src/classes/GuildPartial.ts:8

___

### defaultMessageNotificationsLevel

• **defaultMessageNotificationsLevel**: [`GuildMessageNotificationLevel`](../GuildMessageNotificationLevel/index.md)

#### Defined in

src/classes/Guild.ts:37

___

### deleted

• **deleted**: `boolean` = `false`

#### Defined in

src/classes/Guild.ts:64

___

### description

• **description**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:50

___

### discoverySplashHash

• **discoverySplashHash**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:30

___

### explicitContentFilterLevel

• **explicitContentFilterLevel**: [`GuildExplicitContentFilterLevel`](../GuildExplicitContentFilterLevel/index.md)

#### Defined in

src/classes/Guild.ts:39

___

### features

• **features**: [`GuildFeature`](../modules.md#guildfeature)[]

#### Defined in

src/classes/Guild.ts:41

___

### iconHash

• **iconHash**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:28

___

### id

• `Readonly` **id**: `string`

#### Inherited from

[GuildPartial](../GuildPartial/index.md).[id](../GuildPartial/index.md#id)

#### Defined in

src/classes/GuildPartial.ts:9

___

### isOwner

• **isOwner**: `boolean` = `false`

#### Defined in

src/classes/Guild.ts:31

___

### maxMembers

• **maxMembers**: `undefined` \| `number`

#### Defined in

src/classes/Guild.ts:48

___

### maxPresences

• **maxPresences**: `undefined` \| ``null`` \| `number`

#### Defined in

src/classes/Guild.ts:47

___

### maxVideoChannelUsers

• **maxVideoChannelUsers**: `undefined` \| `number`

#### Defined in

src/classes/Guild.ts:56

___

### members

• **members**: [`GuildMemberManager`](../GuildMemberManager/index.md)

#### Defined in

src/classes/Guild.ts:46

___

### mfaLevel

• **mfaLevel**: [`GuildMFALevel`](../GuildMFALevel/index.md)

#### Defined in

src/classes/Guild.ts:42

___

### name

• **name**: `string`

#### Defined in

src/classes/Guild.ts:27

___

### nsfwLevel

• **nsfwLevel**: [`GuildNSFWLevel`](../GuildNSFWLevel/index.md)

#### Defined in

src/classes/Guild.ts:60

___

### preferredLocale

• **preferredLocale**: `string`

#### Defined in

src/classes/Guild.ts:54

___

### premiumProgressBarEnabled

• **premiumProgressBarEnabled**: `boolean`

#### Defined in

src/classes/Guild.ts:62

___

### premiumSubscriptionCount

• **premiumSubscriptionCount**: `undefined` \| `number`

#### Defined in

src/classes/Guild.ts:53

___

### premiumTier

• **premiumTier**: [`GuildPremiumTierLevel`](../GuildPremiumTierLevel/index.md)

#### Defined in

src/classes/Guild.ts:52

___

### publicUpdatesChannelId

• **publicUpdatesChannelId**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:55

___

### rulesChannelId

• **rulesChannelId**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:45

___

### splashHash

• **splashHash**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:29

___

### stickers

• **stickers**: `undefined` \| `any`[]

#### Defined in

src/classes/Guild.ts:61

___

### systemChannelFlags

• **systemChannelFlags**: [`SystemChannelFlags`](../SystemChannelFlags/index.md)

#### Defined in

src/classes/Guild.ts:44

___

### systemChannelId

• **systemChannelId**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:43

___

### vanityUrlCode

• **vanityUrlCode**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:49

___

### verificationLevel

• **verificationLevel**: [`GuildVerificationLevel`](../GuildVerificationLevel/index.md)

#### Defined in

src/classes/Guild.ts:36

___

### welcomeScreen

• **welcomeScreen**: `any`

#### Defined in

src/classes/Guild.ts:59

___

### widgetChannelId

• **widgetChannelId**: `undefined` \| ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:35

___

### widgetEnabled

• **widgetEnabled**: `undefined` \| `boolean`

#### Defined in

src/classes/Guild.ts:34

## Methods

### edit

▸ **edit**(`options`, `reason?`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](index.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`GuildEditOptions`](../modules.md#guildeditoptions) |
| `reason?` | `string` |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](index.md)\>

#### Defined in

src/classes/Guild.ts:191

___

### fetch

▸ **fetch**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](index.md)\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](index.md)\>

#### Inherited from

[GuildPartial](../GuildPartial/index.md).[fetch](../GuildPartial/index.md#fetch)

#### Defined in

src/classes/GuildPartial.ts:25

___

### isPartial

▸ **isPartial**(): `boolean`

#### Returns

`boolean`

`true` if this is a partial guild, `false` otherwise.

#### Overrides

[GuildPartial](../GuildPartial/index.md).[isPartial](../GuildPartial/index.md#ispartial)

#### Defined in

src/classes/Guild.ts:321
