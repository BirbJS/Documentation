---
layout: default
title: PossibleMemoryLeakWarning
parent: Errors & Warnings
has_toc: true
---

# PossibleMemoryLeakWarning
The PossibleMemoryLeakWarning warning is thrown when Birb.JS detects a situation where a method or function might be causing a memory leak. This is usually used in caches, where options or values you or Birb.JS automatically pass might cause memory leaks or runaway buffers.

## PossibleMemoryLeakWarning: possible memory leak detected!
Birb.JS has detected a situation which might cause a memory leak. You should make sure you're not passing options or parameters that might cause a memory leak, especially if you're using them at scale. An example of this is when you use the `<Cache>.makeSpace()` or `<Cache>.set()` methods whilst setting `options.allowOverflow` to `true`, which forces space to be made by increasing the maximum cache size by 1.

```
PossibleMemoryLeakWarning: possible memory leak detected!
Head to: https://birb.js.org/errors/PossibleMemoryLeakWarning
    at Object.<anonymous> (C:\Users\knokbak\Birb.JS\index.js:20:14)
    at Module._compile (node:internal/modules/cjs/loader:1101:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1153:10)
    at Module.load (node:internal/modules/cjs/loader:981:32)
    at Function.Module._load (node:internal/modules/cjs/loader:822:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:79:12)
    at node:internal/main/run_main_module:17:47
```
