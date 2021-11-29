---
layout: default
title: CacheWarning
parent: Errors & Warnings
has_toc: true
---

# CacheWarning
The CacheWarning warning is a generic warning that is logged to console when something non-critical has gone wrong with the cache.

## CacheWarning: high cache limit provided
You or Birb.JS have set the limit of a [Cache](/classes/Cache) to a very high value. This can cause the cache to be very large and slow down your bot unless you're running a moster of a server. You should consider setting the limit to a lower value if possible.

```
CacheWarning: high cache limit provided
    at Object.<anonymous> (C:\Users\knokbak\Birb.JS\index.js:20:14)
    at Module._compile (node:internal/modules/cjs/loader:1101:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1153:10)
    at Module.load (node:internal/modules/cjs/loader:981:32)
    at Function.Module._load (node:internal/modules/cjs/loader:822:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:79:12)
    at node:internal/main/run_main_module:17:47
```

## CacheWarning: cache overflow detected and allowed by method options: this may lead to a memory leak
You or Birb.JS have set `options.allowOverflow` to `true` whilst calling one of the `<Cache>.makeSpace()` or `<Cache>.set()` methods. The `options.allowOverflow` option is used to allow Birb.JS to make space in the cache if it's full by increasing the cache size limit by 1, which can lead to a memory leak.

```
PossibleMemoryLeakWarning: possible memory leak detected!
Head to: https://birb.js.org/errors/PossibleMemoryLeakWarning
CacheWarning: cache overflow detected and allowed by method options: this may lead to a memory leak
    at Object.<anonymous> (C:\Users\knokbak\Birb.JS\index.js:20:14)
    at Module._compile (node:internal/modules/cjs/loader:1101:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1153:10)
    at Module.load (node:internal/modules/cjs/loader:981:32)
    at Function.Module._load (node:internal/modules/cjs/loader:822:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:79:12)
    at node:internal/main/run_main_module:17:47
```
