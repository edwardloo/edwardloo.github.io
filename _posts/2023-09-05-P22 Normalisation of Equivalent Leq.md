---
title: "Time Correction for Leq"
categories:
    - Blog
tags:
    - Acoustics
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
excerpt: "Quick Note and Example for Leq Normalisation from one reference time to another."
---
# Equivalent Continuous Sound Pressure Level (L_{eq,T})
Basically, the amount of acoustic energy that is lasts continuously throughout measurement time, T, and is equivalent to the actual measured fluctuating sound pressure levels.

## Time Correction for Leq (Normalisation)
The $L_{eq,T}$ of an event that last for time period, T, could be corrected to another reference time, $T_n$ using the following equation:

$$L_{eq,n} = L_{eq,T} + 10\log(\frac{T}{T_n})$$

## Example
Let's say that we have a measured $L_{eq,5s}$ of a single train passby event that last for 5s is 95 dB(A). We would like to obtain the $L_{eq,1hr}$ to assess against authority requirements. Assuming that each hour there would be 10 train passby event on a single train track.
$$L_{eq,1hr} = L_{eq_3600s} = L_{eq,5s} + 10\log(\frac{10(T_5s)}{T_3600s})$$

$$L_{eq,1hr} = 95 + 10\log(\frac{10(5)}{3600})$$

$$L_{eq,1hr} = 95 - 18.6$$

$$L_{eq,1hr} = 76.4 dB(A)$$
---
## References
[1] "*Time Correction*" Jun. 02, 2020. Accessed on Sept. 05, 2023. [Online]. Available: https://strutt.arup.com/help/Fundamentals/TimeRatioAtten.htm
