---
layout: inset
title: Real Time Clock
---

## Introduction

![{{ page.title }}]({{ page.url | | replace: ".html", ".png"}}) 

`(BOOL:IN, DT:PDT) => (BOOL:Q, DT:CDT)`

The real time clock has many uses including time stamping, setting dates and times of day in batch reports, in alarm messages and so on.

### Input

`IN`: The function block is initialized with the specified date and time (at the `PDT` input) by a rising edge at this input.

`PDT`: ( Preset Date and Time ) The initialization values for the function block's date and time. A rising edge at the `IN` input will cause the function block to adopt this value.

### Output

`Q`: If the output is `TRUE` then the values for the date and time at the `CDT` output are valid.

`CDT`: ( Current Date and Time ) The current date and time from the RTC. The CDT output is only updated when the function block is called. For this reason, instances of the function block should be called once in each PLC cycle.

### Example

![Example 1]({{ page.dir }}real-time-clock-example1.png)