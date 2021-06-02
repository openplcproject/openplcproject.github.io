---
layout: inset
title: Semaphore
---

## Introduction

![Semaphore](/reference/standard-function-blocks/semaphore.png)

`( BOOL:CLAIM, BOOL:RELEASE ) => ( BOOL:BUSY )`

This function block provides a mechanism to allow software elements mutually exclusive access to certain resources.
Normally this function is used to synchronize events. 

The `BUSY` output will become `TRUE` once the `CLAIM` input is `TRUE`.  At this point `BUSY` will remain `TRUE` regardless of what the `CLAIM` input is.  

`BUSY` will become `FALSE` when the `RELEASE` input is `TRUE`.
