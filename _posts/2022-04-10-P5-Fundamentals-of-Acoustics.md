---
title: "Fundamental Concepts in Engineering Acoustics"
categories:
    - Blog
tags:
    - Acoustics
---

---
## Definition

> *Acoustics* is defined as the science of sound.

## Sound Characterization (Quantitative vs Qualitative)

| Qualitative (Perceived) | Quantitative (Measured) |
|------------------------|--------------------------|
| Loudness | Sound Pressure Level [dB] |
| Pitch | Frequency [Hz] |
| Duration | Time [s] |

## Sound Level
According to [Weber's Law](https://en.wikipedia.org/wiki/Weber%E2%80%93Fechner_law), perceptions (vision, hearing, taste, touch, and smell) varies logarithmically with the excitation stimulus. Leading to logarithmic expression of sound pressue level.

![image](https://user-images.githubusercontent.com/79191009/162620943-348242c3-7964-4c82-9bd0-857ee01220e5.png)

## Sound Level Weightings
[Frequency weighting](https://www.engineeringtoolbox.com/decibel-d_59.html) system was standardized by the ***International Electrotechnical Commission (IEC)***

| Weighting | Description |
|-----------|-------------|
| A | Initially introduced for low level (loudness) sounds (up to 40 phons). Most commonly used as a rough estimate of the frequency sensitivity of human hearing. |
| B | To treat higher-level (loudness) sound. (Disused) |
| C | Takes better account of low-frequency sound levels. Used in few occupational noise regulations. |
| D | To treat higher-level (loudness) sound. Devoted to aircraft sound level measurements. (Disused) |
| Z (zero) | No weighting. |

For more information, [NTi-Audio](https://www.nti-audio.com/en/support/know-how/frequency-weightings-for-sound-level-measurements) provided a good reference for further reading and correction factors for Octave and 1/3 Octave Bands.

Some reference values on A-weighted SPLs.

| SPL (dBA) | Interpretation |
|-----------|----------------|
| 18 | Woodland area without wind (and without birds singing either! |
| 30 | Empty cinema projection room. |
| 45 | Workstation with the desktop computer fan running. |
| 70 | Busy street. |
| 90 | Airport façade with a plane maneuvering at the pier. |
| 140 | 5 m from a jet engine |

Since it is possible to achieve a given weighted value with rather different spectrum shapes [e.g.: A-weighted SPL for 100 dB (@ 1000 Hz) = 126 dB (@ 63 Hz)], one usually specifies noise limits using simultaneously a global A-weighted sound level value and a frequency contour featuring higher levels in the lower-frequency range than in the higher-frequency range.

### Common Noise Evaluation Contour

| Contour | Description | Standards |
|---------|-------------|-----------|
| [Noise Criterion (NC)](https://www.engineeringtoolbox.com/nc-noise-criterion-d_725.html) | Less stringent, covering frequency range of (62.5 - 8000) Hz | ANSI S12-2-2008 |
| [Noise Rating (NR)](https://www.engineeringtoolbox.com/nr-noise-rating-d_60.html) | More stringent, covering frequency range of (31.5 - 8000) Hz | ISO 1996:1971 |

## Equivalent Sound Levels and Statistical Sound Levels  **pg 5 (23/270)**

![image](https://user-images.githubusercontent.com/79191009/162623803-3256954f-b8f9-42ba-b797-9210472f1b59.png)


---
### References
[1] M. Asselineau, *Building Acoustics*. Boca Raton, Florida: CRC Press, 2015.
