---
layout: default
title: "birb"
has_children: true
has_toc: false
nav_order: 1
---

[birb](README.md) / Exports

# birb

## Table of contents

### Namespaces

- [WebsocketTypes](WebsocketTypes/index.md)

### Enumerations

- [GatewayStatus](GatewayStatus/index.md)
- [GuildExplicitContentFilterLevel](GuildExplicitContentFilterLevel/index.md)
- [GuildMFALevel](GuildMFALevel/index.md)
- [GuildMessageNotificationLevel](GuildMessageNotificationLevel/index.md)
- [GuildNSFWLevel](GuildNSFWLevel/index.md)
- [GuildPremiumTierLevel](GuildPremiumTierLevel/index.md)
- [GuildVerificationLevel](GuildVerificationLevel/index.md)
- [PacketOperation](PacketOperation/index.md)
- [UserNitroType](UserNitroType/index.md)

### Classes

- [APIEndpoint](APIEndpoint/index.md)
- [AuthenticatedAPIEndpoint](AuthenticatedAPIEndpoint/index.md)
- [BaseWebsocket](BaseWebsocket/index.md)
- [Birb](Birb/index.md)
- [BirbAPIError](BirbAPIError/index.md)
- [BirbError](BirbError/index.md)
- [BirbGatewayDisconnection](BirbGatewayDisconnection/index.md)
- [BirbValidationFailedError](BirbValidationFailedError/index.md)
- [Bitfield](Bitfield/index.md)
- [Cache](Cache/index.md)
- [EventDispatcher](EventDispatcher/index.md)
- [EventListener](EventListener/index.md)
- [GetGuildRequest](GetGuildRequest/index.md)
- [Guild](Guild/index.md)
- [GuildMember](GuildMember/index.md)
- [GuildMemberManager](GuildMemberManager/index.md)
- [GuildPartial](GuildPartial/index.md)
- [GuildsManager](GuildsManager/index.md)
- [Intents](Intents/index.md)
- [Manager](Manager/index.md)
- [ModifyGuildRequest](ModifyGuildRequest/index.md)
- [Pair](Pair/index.md)
- [SystemChannelFlags](SystemChannelFlags/index.md)
- [User](User/index.md)
- [UserFlags](UserFlags/index.md)
- [UsersManager](UsersManager/index.md)
- [Websocket](Websocket/index.md)

### Type Aliases

- [APIGuild](modules.md#apiguild)
- [APIGuildMember](modules.md#apiguildmember)
- [APIGuildMemberWithUser](modules.md#apiguildmemberwithuser)
- [APIGuildPartial](modules.md#apiguildpartial)
- [APIResponse](modules.md#apiresponse)
- [APIUser](modules.md#apiuser)
- [AllowedMentionsOptions](modules.md#allowedmentionsoptions)
- [Awaitable](modules.md#awaitable)
- [BirbEvent](modules.md#birbevent)
- [BirbOptions](modules.md#birboptions)
- [BitResolvable](modules.md#bitresolvable)
- [GetGuildParams](modules.md#getguildparams)
- [GuildEditOptions](modules.md#guildeditoptions)
- [GuildFeature](modules.md#guildfeature)
- [IntentsResolvable](modules.md#intentsresolvable)
- [IntentsString](modules.md#intentsstring)
- [MessageMentionTypes](modules.md#messagementiontypes)
- [ModifyGuildParams](modules.md#modifyguildparams)
- [ModifyGuildRequestBody](modules.md#modifyguildrequestbody)
- [SystemChannelFlagsResolvable](modules.md#systemchannelflagsresolvable)
- [SystemChannelFlagsString](modules.md#systemchannelflagsstring)
- [UserFlagsResolvable](modules.md#userflagsresolvable)
- [UserFlagsString](modules.md#userflagsstring)

### Variables

- [IntentFlag](modules.md#intentflag)
- [SystemChannelFlag](modules.md#systemchannelflag)
- [UserFlag](modules.md#userflag)

## Type Aliases

### APIGuild

Ƭ **APIGuild**: `Object`

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `afk_channel_id` | `string` \| ``null`` | id of afk channel |
| `afk_timeout` | `number` | afk timeout in seconds |
| `application_id` | `string` \| ``null`` | application id of the guild creator if it is bot-created |
| `approximate_member_count?` | `number` | approximate number of members in this guild, returned from the `GET /guilds/<id>` endpoint when `with_counts` is `true` |
| `approximate_presence_count?` | `number` | approximate number of non-offline members in this guild, returned from the `GET /guilds/<id>` endpoint when `with_counts` is `true` |
| `banner` | `string` \| ``null`` | banner hash |
| `default_message_notifications` | [`GuildMessageNotificationLevel`](GuildMessageNotificationLevel/index.md) | default message notifications level |
| `description` | `string` \| ``null`` | the description of a guild |
| `discovery_splash` | `string` \| ``null`` | discovery splash hash; only present for guilds with the "DISCOVERABLE" feature |
| `emojis` | `any`[] | custom guild emojis |
| `explicit_content_filter` | [`GuildExplicitContentFilterLevel`](GuildExplicitContentFilterLevel/index.md) | explicit content filter level |
| `features` | [`GuildFeature`](modules.md#guildfeature)[] | enabled guild features |
| `icon` | `string` \| ``null`` | icon hash |
| `id` | `string` | the guild's id |
| `max_members?` | `number` | the maximum number of members for the guild |
| `max_presences?` | `number` \| ``null`` | the maximum number of presences for the guild (`null` is always returned, apart from the largest of guilds) |
| `max_video_channel_users?` | `number` | the maximum amount of users in a video channel |
| `mfa_level` | [`GuildMFALevel`](GuildMFALevel/index.md) | required MFA level for the guild |
| `name` | `string` | guild name (2-100 characters, excluding trailing and leading whitespace) |
| `nsfw_level` | [`GuildNSFWLevel`](GuildNSFWLevel/index.md) | guild NSFW level |
| `owner?` | `boolean` | true if the user is the owner of the guild |
| `owner_id` | `string` | id of owner |
| `permissions?` | `string` | total permissions for the user in the guild (excludes overwrites) |
| `preferred_locale` | `string` | the preferred locale of a Community guild; used in server discovery and notices from Discord, and sent in interactions; defaults to `en-US` |
| `premium_progress_bar_enabled` | `boolean` | whether the guild has the boost progress bar enabled |
| `premium_subscription_count?` | `number` | the number of boosts this guild currently has |
| `premium_tier` | [`GuildPremiumTierLevel`](GuildPremiumTierLevel/index.md) | premium tier (Server Boost level) |
| `public_updates_channel_id` | `string` \| ``null`` | the id of the channel where admins and moderators of Community guilds receive notices from Discord |
| `roles` | `any`[] | roles in the guild |
| `rules_channel_id` | `string` \| ``null`` | the id of the channel where Community guilds can display rules and/or guidelines |
| `splash` | `string` \| ``null`` | splash hash |
| `stickers?` | `any`[] | custom guild stickers |
| `system_channel_flags` | `number` | system channel flags |
| `system_channel_id` | `string` \| ``null`` | the id of the channel where guild notices such as welcome messages and boost events are posted |
| `vanity_url_code` | `string` \| ``null`` | the vanity url code for the guild |
| `verification_level` | [`GuildVerificationLevel`](GuildVerificationLevel/index.md) | verification level required for the guild |
| `welcome_screen?` | `any` | the welcome screen of a Community guild, shown to new members, returned in an Invite's guild object |
| `widget_channel_id` | `string` \| ``null`` | the channel id that the widget will generate an invite to, or null if set to no invite |
| `widget_enabled?` | `boolean` | true if the server widget is enabled |

#### Defined in

src/classes/api/types/APIGuild.ts:1

___

### APIGuildMember

Ƭ **APIGuildMember**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `avatar?` | `string` \| ``null`` |
| `communication_disabled_until?` | `string` \| ``null`` |
| `deaf` | `boolean` |
| `joined_at` | `string` |
| `mute` | `boolean` |
| `nick?` | `string` \| ``null`` |
| `pending?` | `boolean` |
| `premium_since?` | `string` \| ``null`` |
| `roles` | `string`[] |

#### Defined in

src/classes/api/types/APIGuildMember.ts:3

___

### APIGuildMemberWithUser

Ƭ **APIGuildMemberWithUser**: [`APIGuildMember`](modules.md#apiguildmember) & { `user`: [`APIUser`](modules.md#apiuser)  }

#### Defined in

src/classes/api/types/APIGuildMember.ts:15

___

### APIGuildPartial

Ƭ **APIGuildPartial**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `unavailable?` | `boolean` |

#### Defined in

src/classes/api/types/APIGuild.ts:160

___

### APIResponse

Ƭ **APIResponse**<`Type`\>: `Object`

#### Type parameters

| Name | Type |
| :------ | :------ |
| `Type` | `any` |

#### Type declaration

| Name | Type |
| :------ | :------ |
| `json` | `Type` |
| `status` | `number` |

#### Defined in

src/classes/api/APIEndpoint.ts:143

___

### APIUser

Ƭ **APIUser**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `avatar` | `string` \| ``null`` |
| `banner?` | `string` \| ``null`` |
| `bot?` | `boolean` |
| `discriminator` | `string` |
| `email?` | `string` \| ``null`` |
| `flags?` | `number` |
| `id` | `string` |
| `locale?` | `string` |
| `mfa_enabled?` | `boolean` |
| `premium_type?` | [`UserNitroType`](UserNitroType/index.md) |
| `public_flags?` | `number` |
| `system?` | `boolean` |
| `username` | `string` |
| `verified?` | `boolean` |

#### Defined in

src/classes/api/types/APIUser.ts:1

___

### AllowedMentionsOptions

Ƭ **AllowedMentionsOptions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `parse?` | [`MessageMentionTypes`](modules.md#messagementiontypes)[] |
| `repliedUser?` | `boolean` |
| `roles?` | `string`[] |
| `users?` | `string`[] |

#### Defined in

src/classes/Birb.ts:173

___

### Awaitable

Ƭ **Awaitable**<`T`\>: `Promise`<`T`\> \| `T`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Defined in

src/utils/types.ts:1

___

### BirbEvent

Ƭ **BirbEvent**: ``"ready"`` \| ``"guildCreate"`` \| ``"guildUpdate"`` \| ``"guildUnavailable"`` \| ``"guildDelete"`` \| ``"gatewayConnectionEstablished"`` \| ``"websocketHeartbeatSent"`` \| ``"websocketHeartbeatAckReceived"`` \| ``"packetSent"`` \| ``"packetReceived"``

#### Defined in

src/classes/Birb.ts:180

___

### BirbOptions

Ƭ **BirbOptions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `allowedMentions?` | [`AllowedMentionsOptions`](modules.md#allowedmentionsoptions) |
| `debug?` | `boolean` |
| `intents` | [`IntentsResolvable`](modules.md#intentsresolvable)[] |

#### Defined in

src/classes/Birb.ts:167

___

### BitResolvable

Ƭ **BitResolvable**<`Flags`\>: `Flags` \| `bigint`

#### Type parameters

| Name |
| :------ |
| `Flags` |

#### Defined in

src/classes/bitfields/Bitfield.ts:3

___

### GetGuildParams

Ƭ **GetGuildParams**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `guildId` | `string` |
| `withCounts?` | `boolean` |

#### Defined in

src/classes/api/endpoints/GetGuildRequest.ts:7

___

### GuildEditOptions

Ƭ **GuildEditOptions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `afkChannelId?` | `string` \| ``null`` |
| `afkTimeout?` | ``60`` \| ``300`` \| ``900`` \| ``1800`` \| ``3600`` |
| `defaultMessageNotificationsLevel?` | [`GuildMessageNotificationLevel`](GuildMessageNotificationLevel/index.md) |
| `description?` | `string` \| ``null`` |
| `explicitContentFilterLevel?` | [`GuildExplicitContentFilterLevel`](GuildExplicitContentFilterLevel/index.md) |
| `features?` | [`GuildFeature`](modules.md#guildfeature)[] |
| `name?` | `string` |
| `ownerId?` | `string` |
| `preferredLocale?` | `string` |
| `premiumProgressBarEnabled?` | `boolean` |
| `publicUpdatesChannelId?` | `string` \| ``null`` |
| `rulesChannelId?` | `string` \| ``null`` |
| `systemChannelFlags?` | [`SystemChannelFlagsResolvable`](modules.md#systemchannelflagsresolvable)[] |
| `systemChannelId?` | `string` \| ``null`` |
| `verificationLevel?` | [`GuildVerificationLevel`](GuildVerificationLevel/index.md) |

#### Defined in

src/classes/Guild.ts:326

___

### GuildFeature

Ƭ **GuildFeature**: ``"ANIMATED_BANNER"`` \| ``"ANIMATED_ICON"`` \| ``"AUTO_MODERATION"`` \| ``"BANNER"`` \| ``"COMMUNITY"`` \| ``"DISCOVERABLE"`` \| ``"FEATURABLE"`` \| ``"INVITE_SPLASH"`` \| ``"MEMBER_VERIFICATION_GATE_ENABLED"`` \| ``"MONETIZATION_ENABLED"`` \| ``"MORE_STICKERS"`` \| ``"NEWS"`` \| ``"PARTNERED"`` \| ``"PREVIEW_ENABLED"`` \| ``"PRIVATE_THREADS"`` \| ``"ROLE_ICONS"`` \| ``"TICKETED_EVENTS_ENABLED"`` \| ``"VANITY_URL"`` \| ``"VERIFIED"`` \| ``"VIP_REGIONS"`` \| ``"WELCOME_SCREEN_ENABLED"``

#### Defined in

src/classes/api/types/APIGuild.ts:203

___

### IntentsResolvable

Ƭ **IntentsResolvable**: [`BitResolvable`](modules.md#bitresolvable)<[`IntentsString`](modules.md#intentsstring)\>

#### Defined in

src/classes/bitfields/Intents.ts:4

___

### IntentsString

Ƭ **IntentsString**: keyof typeof [`IntentFlag`](modules.md#intentflag)

#### Defined in

src/classes/bitfields/Intents.ts:3

___

### MessageMentionTypes

Ƭ **MessageMentionTypes**: ``"users"`` \| ``"roles"`` \| ``"everyone"``

#### Defined in

src/utils/types.ts:2

___

### ModifyGuildParams

Ƭ **ModifyGuildParams**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `guildId` | `string` |

#### Defined in

src/classes/api/endpoints/ModifyGuildRequest.ts:11

___

### ModifyGuildRequestBody

Ƭ **ModifyGuildRequestBody**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `afk_channel_id?` | `string` \| ``null`` |
| `afk_timeout?` | `number` |
| `default_message_notifications?` | [`GuildMessageNotificationLevel`](GuildMessageNotificationLevel/index.md) |
| `description?` | `string` \| ``null`` |
| `explicit_content_filter?` | [`GuildExplicitContentFilterLevel`](GuildExplicitContentFilterLevel/index.md) |
| `features?` | [`GuildFeature`](modules.md#guildfeature)[] |
| `name?` | `string` |
| `owner_id?` | `string` |
| `preferred_locale?` | `string` |
| `premium_progress_bar_enabled?` | `boolean` |
| `public_updates_channel_id?` | `string` \| ``null`` |
| `rules_channel_id?` | `string` \| ``null`` |
| `system_channel_flags?` | `bigint` |
| `system_channel_id?` | `string` \| ``null`` |
| `verification_level?` | [`GuildVerificationLevel`](GuildVerificationLevel/index.md) |

#### Defined in

src/classes/api/endpoints/ModifyGuildRequest.ts:15

___

### SystemChannelFlagsResolvable

Ƭ **SystemChannelFlagsResolvable**: [`BitResolvable`](modules.md#bitresolvable)<[`SystemChannelFlagsString`](modules.md#systemchannelflagsstring)\>

#### Defined in

src/classes/bitfields/SystemChannelFlags.ts:4

___

### SystemChannelFlagsString

Ƭ **SystemChannelFlagsString**: keyof typeof [`SystemChannelFlag`](modules.md#systemchannelflag)

#### Defined in

src/classes/bitfields/SystemChannelFlags.ts:3

___

### UserFlagsResolvable

Ƭ **UserFlagsResolvable**: [`BitResolvable`](modules.md#bitresolvable)<[`UserFlagsString`](modules.md#userflagsstring)\>

#### Defined in

src/classes/bitfields/UserFlags.ts:4

___

### UserFlagsString

Ƭ **UserFlagsString**: keyof typeof [`UserFlag`](modules.md#userflag)

#### Defined in

src/classes/bitfields/UserFlags.ts:3

## Variables

### IntentFlag

• `Const` **IntentFlag**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `AUTO_MODERATION_CONFIGURATION` | `bigint` |
| `AUTO_MODERATION_EXECUTION` | `bigint` |
| `DIRECT_MESSAGES` | `bigint` |
| `DIRECT_MESSAGE_REACTIONS` | `bigint` |
| `DIRECT_MESSAGE_TYPING` | `bigint` |
| `GUILDS` | `bigint` |
| `GUILD_BANS` | `bigint` |
| `GUILD_EMOJIS_AND_STICKERS` | `bigint` |
| `GUILD_INTEGRATIONS` | `bigint` |
| `GUILD_INVITES` | `bigint` |
| `GUILD_MEMBERS` | `bigint` |
| `GUILD_MESSAGES` | `bigint` |
| `GUILD_MESSAGE_REACTIONS` | `bigint` |
| `GUILD_MESSAGE_TYPING` | `bigint` |
| `GUILD_PRESENCES` | `bigint` |
| `GUILD_SCHEDULED_EVENTS` | `bigint` |
| `GUILD_VOICE_STATES` | `bigint` |
| `GUILD_WEBHOOKS` | `bigint` |
| `MESSAGE_CONTENT` | `bigint` |

#### Defined in

src/classes/bitfields/Intents.ts:5

___

### SystemChannelFlag

• `Const` **SystemChannelFlag**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `SUPPRESS_GUILD_REMINDER_NOTIFICATIONS` | `bigint` |
| `SUPPRESS_JOIN_NOTIFICATIONS` | `bigint` |
| `SUPPRESS_JOIN_NOTIFICATION_REPLIES` | `bigint` |
| `SUPPRESS_PREMIUM_SUBSCRIPTIONS` | `bigint` |

#### Defined in

src/classes/bitfields/SystemChannelFlags.ts:6

___

### UserFlag

• `Const` **UserFlag**: `Object`

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `BOT_HTTP_INTERACTIONS` | `bigint` | A bot that uses only [HTTP interactions](https://discord.com/developers/docs/interactions/receiving-and-responding#receiving-an-interaction) and is shown in the online member list |
| `BUG_HUNTER_LEVEL_1` | `bigint` | Bug Hunter Level 1 |
| `BUG_HUNTER_LEVEL_2` | `bigint` | Bug Hunter Level 2 |
| `CERTIFIED_MODERATOR` | `bigint` | Discord Certified Moderator |
| `HYPESQUAD` | `bigint` | HypeSquad Events Member |
| `HYPESQUAD_ONLINE_HOUSE_BALANCE` | `bigint` | House Balance Member |
| `HYPESQUAD_ONLINE_HOUSE_BRAVERY` | `bigint` | House Bravery Member |
| `HYPESQUAD_ONLINE_HOUSE_BRILLIANCE` | `bigint` | House Brilliance Member |
| `NITRO_EARLY_SUPPORTER` | `bigint` | Early Nitro Supporter |
| `PARTNER` | `bigint` | Partnered Server Owner |
| `STAFF` | `bigint` | Discord Employee or Staff Member |
| `TEAM_PSEUDO_USER` | `bigint` | The user is actually a [team](https://discord.com/developers/docs/topics/teams) |
| `VERIFIED_BOT` | `bigint` | Verified Bot |
| `VERIFIED_BOT_DEVELOPER` | `bigint` | Early Verified Bot Developer |

#### Defined in

src/classes/bitfields/UserFlags.ts:5
