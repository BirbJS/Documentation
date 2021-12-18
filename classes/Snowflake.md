---
layout: default
title: Snowflake
parent: Classes
has_children: false
has_toc: true
---

# Snowflake
### Table of Contents
{: .no_toc .text-delta }

- TOC
{:toc}
# Constructor
```js
new Snowflake(epoch)
```

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| epoch | *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)* or bigint or Date | the epoch to use
 | false | *none* |

# Properties
## decode
**Type:** *[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)*

# Methods
## deconstruct(id)
Deconstructs a snowflake given a snowflake ID

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| id | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* or bigint | the snowflake to deconstruct | false | *none* |

**Returns:** DeconstructedSnowflake

## generate(options?)
Generates a snowflake given an epoch and optionally a timestamp

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| options | SnowflakeGenerateOptions | options to pass into the generator, see {@link SnowflakeGenerateOptions}

**note** when `increment` is not provided it defaults to the private `increment` of the instance | true | *none* |

**Returns:** bigint

## timestampFrom(id)
Retrieves the timestamp field's value from a snowflake.

| name | type | description | optional | default |
|:-----|:-----|:------------|:---------|:--------|
| id | *[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string)* or bigint | The snowflake to get the timestamp value from. | false | *none* |

**Returns:** *[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/number)*

