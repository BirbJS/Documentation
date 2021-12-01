---
layout: default
title: CacheError
parent: Errors & Warnings
has_toc: true
---

# CacheError
The CacheError error is a generic error that is thrown when something has gone wrong with the cache.

## CacheError: cannot write to cache; no available resolution provided in makeCache.options; cache is full
Birb.JS is unable to write to the cache because the cache is full and no resolution (like removing the oldest entry) has been provided in `makeCache.options`.

```
CacheError: cannot write to cache; no available resolution provided in makeCache.options; cache is full
    at Object.<anonymous> (C:\Users\knokbak\Birb.JS\index.js:20:14)
    at Module._compile (node:internal/modules/cjs/loader:1101:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1153:10)
    at Module.load (node:internal/modules/cjs/loader:981:32)
    at Function.Module._load (node:internal/modules/cjs/loader:822:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:79:12)
    at node:internal/main/run_main_module:17:47
```
