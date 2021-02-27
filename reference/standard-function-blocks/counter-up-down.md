---
layout: inset
title: Counter Up-Down
---

## Introduction

The up-down counter can be used to both increment and decrement the same counter variable `CV`.
A pulse on the reset input `R` resets the value of `CV` to 0. 
A pulse on the maximum value `PV` will initialize `CV` to `PV`.
Each time the input `CU` is set to `TRUE`, `CV` is incremented by 1, provided that `CV` is less than the maximum value `PV`.
Each time the input `CD` is set to `TRUE`, `CV` is decremented by 1, provided that `CV` is greater than 0.
The output `QU` is set to `TRUE` when `CV` is greater than or equal to `PV`. 
The output `QD` is set to `TRUE` when `CV` is is less than or equal to 0. 
