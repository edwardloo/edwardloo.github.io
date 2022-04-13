---
title: "Basics of Reverberation Time"
categories:
    - Blog
tags:
    - Acoustics
    - Noise Control
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
---

---
## Reverberation

> ***Reverberation*** is the persistence of sound in an enclosed volume due to multiple reflections on the enclosed surfaces after the sound source has been stopped. Reverberation is usually quantified as reverberation time, *T60*.

<img src = "https://user-images.githubusercontent.com/79191009/163111136-ed305da3-62eb-4535-8e8f-56bc00c5be36.png" width = 400 height = 250>{: .align-center}

Figure 1: Reverberation  due to Acoustic Reflections in Enclosed Space (Source: [1])
{: .text-center}

### Absorption Coefficient, *α*

When sound wave impinges on a material, part of the energy will be reflected, another part will be transmitted through, and the last part will be absorbed as heat loss aas shown in Figure 2. Absorption coefficient is used to quantify the transmitted and absorbed part when sound wave strikes a material.

<img src = "https://user-images.githubusercontent.com/79191009/163110690-d4bd4e1d-bd80-43f1-8835-fe6ff3accc48.png" weidth = 300 height = 300>{: .align-center}

Figure 2: Incident (*Ii*), reflected (*Ir*), Absorbed (*Ia*), and Transmitted (*It*) Waves (Source: [1])
{: .text-center}

> ***Absorption coefficient*** is defined as the ratio of absorbed energy over incident energy.

![image](https://user-images.githubusercontent.com/79191009/163108917-8bffe3d1-6511-4739-bbcd-d79ae89e9306.png){: .align-center}

Where :
  - *A* = equivalent absorption area
  - *S* = surface area
  - *α* = absorption coefficient

More information on *α* :
  - *α* range from 0 to 1
  - *α* is frequency dependent
  - material are considered absorptive is *α* > 0.5
  - thicker materials have better absorptive performance in low-frequency range
  - absorptive material usually low high airflow resistivity

### Reverberation vs Echo

| Parameter | Reverberation | Echo |
|-----------|---------------|------|
| Intuition | Similar to time constant of a physical system; the response after providing an impluse excitation | Product of multiple reflections that last a very short time span (no longer than 22 ms) which arrived well after the direct sound (i.e., more than 100 ms) |
| Perception | Perceived continuously by listener | Perceived as discrete sounds |
| Example Response of "Hi" | "Hhhhhiiiiiiiiiii..." | "Hi"..."Hi"..."Hi"... |

## Reverberation Time, *T60*

> Reverberation time (RT) is defined as the time taken for a sound source level to decay by 60 *dB* afterthe sound source is stopped across frequency bands. RT is frequency dependent.

Sometimes, a change of slope could be observed in a reverberation curve which usually indicates the presence of a [flutter echo](https://www.supawood.com.au/news/architecturally-sound-part-2-how-flutter-echo-impacts-a-space).

<img src = "https://user-images.githubusercontent.com/79191009/163113860-3db9c66c-1255-4684-812c-15e42a0f6c6b.png" width = 550 height = 400>{: .align-center}

Figure 3: Example of Reverberation Time Curve with Flutter Echo (Source: [1])
{: .text-center}

### Reverberation Time Design Standards

| Standard | Title |
|----------|----------|
| AS/NZS 2107:2016 | Acoustics-Recommended Design Sound Levels and Reverberation Times for Building Interiors |

### Reverberation Time Measurement

1. Creating a sufficiently loud noise (usually > 90 *dB*) either by impulse noise (e.g.: blan pistol shot/balloon burst) or random noise signal ([pink](https://en.wikipedia.org/wiki/Pink_noise)/[white](https://en.wikipedia.org/wiki/White_noise) noise)
2. Measure the response of the enclosed space using a calibrated sound level meter (response time set to *impulse* option)
3. Plot the response across different octave bands to obtain the time  taken for 60 *dB* drop
4. If the decay of 60 *dB* is not attainable (occurs frequently), extrapolation from ***T20*** or ***T30*** could be used as well, given that the decay is linear

| Extrapolation Method | *T30* | *T20* |
|----------------------|-------|-------|
| Equation | ***T60 ≈ 2(T30)*** | ***T60 ≈ 3(T20)*** |

### Reverberation Time Measurement Standards

| Standard | Scenario |
|----------|----------|
| ISO 3382-1 | standard for performance spaces |
| ISO 3382-2 | standard for ordinary rooms |
| ISO 3382-3 | standard for open-plan offices |
| ASTM E2235 | standard for use in sound insulation |

## Reverberation Time Computations

### Sabine Equation

![image](https://user-images.githubusercontent.com/79191009/163117231-86dca260-6910-4062-b52e-4f3375eea028.png){: .align-center}

Where :
  - *c20* = speed of sound at 20 °C [*m/s^2*]
  - *V* =   the volume of enclosed space [*m^3*]
  - *S* =   the total surface area of enclosed space [*m^2*]
  - *α* =   the average absorption coefficient of room surfaces
  - *Sα* =  the total absorption [*sabins*]

Sabine equation :
  - assumed that the enclosed volumes have rather reflective surfaces with similar dimensions ("live" rooms)
  - tends to over-predict reverberation time for small rooms with high amounts of absorption
  - will perform poorly (low accuracy) when the absorption is larger
  - only valid for uniform volumes like cuboid

### Eyring Equation

![image](https://user-images.githubusercontent.com/79191009/163118609-d801a5f3-c1f9-46f6-972d-1a9340145a3d.png){: .align-center}

Eyring equation :
  - better estimates the RT in small rooms with relatively large quantities of sound absorption ("dead" rooms)
  - approximates to Sabine equation for very "live" rooms
  - usually used for recording studios or critical listening environments

## Spatial Sound Level Decay

Although reverberation time is widely used, it is not always the best for describing internal acoustics. For example:

> A flat encumbered space it will feature a rather low value, sometimes similar to that for a small lounge, while people inside will find the acoustics uncomfortable.

For such situations, one may use the spatial sound level decay *DL2*, which is the rate of sound level decay with doubling of distance. As shown in Figure 4, it is possible to distinguish the direct field region close to the source (where the influence of the room is not yet felt) and the far field region (where one is left with the reverberant field). In between stands the intermediate region, which is controlled by the acoustic treatment of the room.


<img src ="https://user-images.githubusercontent.com/79191009/163113531-0a7375a4-4478-473d-bd6c-83a0b74cfd98.png" width = 550 height = 400>{: .align-center}

Figure 4: Spatial Sound Level Decay Curve (Source: [1])
{: .text-center}

---
## References
[1] M. Asselineau, *Building Acoustics*. Boca Raton, Florida: CRC Press, 2015.

[2] D. A. Bies, C. H. Hansen, and C. Q. Howard, *Engineering Noise Control*, 5th ed. Boca Raton, Florida: CRC Press, 2017.

[3] Wikipedia, *Reverberation*, Wikipedia, Jan. 10, 2022. Accessed on: Apr. 13, 2022. [Online]. Available: https://en.wikipedia.org/wiki/Reverberation
