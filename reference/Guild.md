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
- [premiumProgressBarEnabled](Guild.md#premiumprogressbarenabled)
- [premiumSubscriptionCount](Guild.md#premiumsubscriptioncount)
- [premiumTier](Guild.md#premiumtier)
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

[GuildPartial](GuildPartial.md).[available](GuildPartial.md#available)

#### Defined in

src/classes/Guild.ts:63

___

### bannerHash

• **bannerHash**: ``null`` \| `string`

#### Defined in

src/classes/Guild.ts:51

___

### client

• **client**: [`Birb`](Birb.md)

#### Inherited from

[GuildPartial](GuildPartial.md).[client](GuildPartial.md#client)

#### Defined in

src/classes/GuildPartial.ts:8

___

### defaultMessageNotificationsLevel

• **defaultMessageNotificationsLevel**: [`GuildMessageNotificationLevel`](GuildMessageNotificationLevel.md)

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

• **explicitContentFilterLevel**: [`GuildExplicitContentFilterLevel`](GuildExplicitContentFilterLevel.md)

#### Defined in

src/classes/Guild.ts:39

___

### features

• **features**: [`GuildFeature`](modules.md#guildfeature)[]

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

[GuildPartial](GuildPartial.md).[id](GuildPartial.md#id)

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

• **members**: [`GuildMemberManager`](GuildMemberManager.md)

#### Defined in

src/classes/Guild.ts:46

___

### mfaLevel

• **mfaLevel**: [`GuildMFALevel`](GuildMFALevel.md)

#### Defined in

src/classes/Guild.ts:42

___

### name

• **name**: `string`

#### Defined in

src/classes/Guild.ts:27

___

### nsfwLevel

• **nsfwLevel**: [`GuildNSFWLevel`](GuildNSFWLevel.md)

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

• **premiumTier**: [`GuildPremiumTierLevel`](GuildPremiumTierLevel.md)

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

• **systemChannelFlags**: [`SystemChannelFlags`](SystemChannelFlags.md)

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

• **verificationLevel**: [`GuildVerificationLevel`](GuildVerificationLevel.md)

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

▸ **edit**(`options`, `reason?`): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`GuildEditOptions`](modules.md#guildeditoptions) |
| `reason?` | `string` |

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Defined in

src/classes/Guild.ts:191

___

### fetch

▸ **fetch**(): [`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Returns

[`Promise`]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise )<[`Guild`](Guild.md)\>

#### Inherited from

[GuildPartial](GuildPartial.md).[fetch](GuildPartial.md#fetch)

#### Defined in

src/classes/GuildPartial.ts:25

___

### isPartial

▸ **isPartial**(): `boolean`

#### Returns

`boolean`

`true` if this is a partial guild, `false` otherwise.

#### Overrides

[GuildPartial](GuildPartial.md).[isPartial](GuildPartial.md#ispartial)

#### Defined in

src/classes/Guild.ts:321
