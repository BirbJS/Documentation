---
layout: default
title: WebsocketTypes
parent: Namespaces
grand_parent: Reference
has_toc: false
nav_order: 1
---

[Birb](/) / WebsocketTypes

# Namespace: WebsocketTypes

## Table of contents

### Type Aliases

- [GatewayGuildCreateData](WebsocketTypes.md#gatewayguildcreatedata)
- [GatewayGuildDeleteData](WebsocketTypes.md#gatewayguilddeletedata)
- [GatewayGuildUpdateData](WebsocketTypes.md#gatewayguildupdatedata)

## Type Aliases

### GatewayGuildCreateData

Ƭ **GatewayGuildCreateData**: [`APIGuild`](modules.md#apiguild) & { `channels`: `any`[] ; `guild_scheduled_events`: `any`[] ; `joined_at`: `string` ; `large`: `boolean` ; `member_count`: `number` ; `members`: `any`[] ; `presences`: `any`[] ; `stage_instances`: `any`[] ; `threads`: `any`[] ; `unavailable?`: `boolean` ; `voice_states`: `any`[]  }

#### Defined in

src/classes/ws/types.ts:3

___

### GatewayGuildDeleteData

Ƭ **GatewayGuildDeleteData**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `unavailable?` | `boolean` |

#### Defined in

src/classes/ws/types.ts:19

___

### GatewayGuildUpdateData

Ƭ **GatewayGuildUpdateData**: [`APIGuild`](modules.md#apiguild)

#### Defined in

src/classes/ws/types.ts:17
