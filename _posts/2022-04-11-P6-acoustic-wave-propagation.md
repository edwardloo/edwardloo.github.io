---
title: "Acoustic Wave Propagation"
categories:
    - Blog
tags:
    - Acoustics  
---

---
## Free Field Acoustic Wave Propagation

> *Acoustic free field* is a situation where there are no obstacle is close to the sound source, the receiver, and the sound path.

Under free field condition:
  - Sound wave from **omnidirectional** point sound source will be **spherical**
  - Sound pressure level, *Lp*, is a function of sound power level, *Lw*, of the source and the distance, *d*, from the source to receptor.

![image](https://user-images.githubusercontent.com/79191009/162658079-5c18606a-3dd3-4991-9f45-b69fc5bb55eb.png)

Where *Q* is the directivity factor of the source:

| *Q* | Type of source | Directivity Index, *DI* (dB) | # of Reflective surface |
|-----|----------------|------------------------------|-------------------------|
| 1 | omnidirectional source | 0 | None |
| 2 | omnidirectional source over a reflective plane | 3 | 1 |
| 4 | omnidirectional source in a corner of 2 reflective plane | 6 | 2 |
| 8 | omnidirectional source in a corner of 3 reflective plane | 9 | 3 |

and *D* is the extra attenuation (e.g.: barriers, ground effects etc.):

## Types of Wave Propagation Situations

| Situation | Remark | Attenuation Term | Standard |
|-----------|--------|------------------|----------|
| Terrain (ground effect) | Complicates calculation through screening or reflection | ![image](https://user-images.githubusercontent.com/79191009/162659562-42988c05-7458-4e54-915c-337037503fac.png) |  (ISO 9613) |
| Room (very small) | All dimensions are small compared to wavelength of sound source | Stationary waves | - |
| Room (normal) | Free path is large compared to wavelength of sound source (practically constant reverberant field) | ![image](https://user-images.githubusercontent.com/79191009/162660078-0b18f7b1-6136-4686-9db5-31f201dd5a74.png) | - |
| Room (very large) | Spatial sound level decay is present | Empirical model exists, but usage of simulation models are advised | - |

Where:

- *h_m* = the average height above ground of the direct sound propagation path, in m
- *α* = mean absorption coefficient
- *A* = total area of absorption, in m^2

---
### References
[1] M. Asselineau, *Building Acoustics*. Boca Raton, Florida: CRC Press, 2015.

[2] D. A. Bies, C. H. Hansen, and C. Q. Howard, *Engineering Noise Control*, 5th ed. Boca Raton, Florida: CRC Press, 2017.
