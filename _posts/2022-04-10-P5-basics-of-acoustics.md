---
title: "Basic Concepts in Engineering Acoustics"
categories:
    - Blog
tags:
    - Acoustics
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
---

---
## Definition

> *Acoustics* is defined as the science of sound.

## Sound Characterization

| Qualitative (Perceived) | Quantitative (Measured) |
|------------------------|--------------------------|
| Loudness | Sound Pressure Level [dB] |
| Pitch | Frequency [Hz] |
| Duration | Time [s] |

## Sound Level
According to [Weber's Law](https://en.wikipedia.org/wiki/Weber%E2%80%93Fechner_law), perceptions (vision, hearing, taste, touch, and smell) varies logarithmically with the excitation stimulus. Leading to logarithmic expression of sound pressue level.

![image](https://user-images.githubusercontent.com/79191009/162620943-348242c3-7964-4c82-9bd0-857ee01220e5.png){: .align-center}

### Human Hearing Threshold

| Parameter | Lower Limit | Upper Limit |
|-----------|-------------|-------------|
| Pressure | 20 μPa (Threshold of Hearing) | 200 Pa (Threshold of Pain) |
| SPL (ref 20 μPa) | 0 dB | 140 dB |
| Frequency | 20 Hz | 20,000 Hz |
| Most Sensitive *f* (Human) | 500 Hz | 5,000 Hz |

### Human Perception of SPL in dB

| Change in SPL (dB) | Loudness Perceived |
|--------------------|--------------------|
| 3 | Perceivable |
| 5 | Noticeable difference |
| 10 | Twice as loud|
| 15 | Significant difference |
| 20 | Four times as loud |

### Addition of SPL
![image](https://user-images.githubusercontent.com/79191009/162629886-8655f658-8232-4070-9fbb-4faa28105508.png){: .align-center}

| X +  (dB): | Result (dB) |
|------------|--------|
| X | X + 3 |
| X + 1 | X + 3.5 |
| X + 2 | X + 4.1 |
| X + 3 | X + 4.8 |
| X + 4 | X + 5.5 |
| X + 5 | X + 6.2 |
| X + 6 | X + 7.0 |
| X + 7 | X + 7.8 |
| X + 8 | X + 8.6 |
| X + 9 | X + 9.5 |
| X + 10 | X + 10.4 |
| X + 11 | X + 11.3 |
| X + 12 | X + 12.3 |
| X + 13 | X + 13.2 |
| X + 14 | X + 14.2 |
| X + 15 | X + 15.1 |
| X + 16 | X + 16.1 |

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

Since it is possible to achieve a given weighted value with rather different spectrum shapes, one usually specifies noise limits using simultaneously a global A-weighted sound level value and a frequency contour featuring higher levels in the lower-frequency range than in the higher-frequency range.

> E.g.: A-weighted SPL for 100 dB (@ 1000 Hz) = 126 dB (@ 63 Hz)

### Common Noise Weighting Curves (Countours)

| Contour | Description | Standards |
|---------|-------------|-----------|
| [Noise Criterion (NC)](https://www.engineeringtoolbox.com/nc-noise-criterion-d_725.html) | Less stringent, covering frequency range of (62.5 - 8000) Hz | ANSI S12-2-2008 |
| [Noise Rating (NR)](https://www.engineeringtoolbox.com/nr-noise-rating-d_60.html) | More stringent, covering frequency range of (31.5 - 8000) Hz | ISO 1996:1971 |

## Equivalent Sound Levels and Statistical Sound Levels

### Equivalent Sound Pressure Level, <img src="https://user-images.githubusercontent.com/79191009/162631815-8de8d7a7-a0e1-43cc-836f-71a53cf851ac.png" width="40" height="30">

Acoustic measurements are temporal fluctuations of pressure. To gauge or quantify the measurements easily, equivalent sound level, *Leq*, is used. For A-weighted *Leq*, the quantity is denoted as *LAeq*.

> Leq represents a non-fluctuating signal containing as much acoustic energy as the signal under study over the period of time considered.

![image](https://user-images.githubusercontent.com/79191009/162632102-8b8e358f-ab3c-4541-9f06-7b25a57659b0.png)
(Source: [*NI Sound and Vibration Software: Leq Sound Level Meaning*](https://knowledge.ni.com/KnowledgeArticleDetails?id=kA00Z0000019N3eSAE))

### Statistical Sound Level, <img src="https://user-images.githubusercontent.com/79191009/162632837-a1265604-8124-4d62-9059-5f652d874adb.png" width="40" height="30">

> In actual, a 65 dB(A) *LAeq* value can be reached close to a major highway where it is a continuous rumble, but it can also be reached close to a country road if a single motorcycle passes by

Although with *Leq*, it is easier to make sense of the acoustic measurements, the temporal fluctuations of a noise could be very different with the same *Leq*. This is when people use the notion of statistical sound levels, *Lx*.

> *Lx* is the sound level reached or exceeded for *x %* of the analysis time.

Commonly used *Lx* values are:

| *Lx* | Meaning | Interpretation |
|------|---------|----------------|
| *L10* | Sound level reached or exceeded for *10%* of the analysis time. | Quantify the highest noise level taken. Used for measuring impact or short and transient burst of noise (e.g.: traffic noise). |
| *L50* | Sound level reached or exceeded for *50%* of the analysis time. | Usually less than *Leq* for fluctuating noise. |
| *L90* | Sound level reached or exceeded for *90%* of the analysis time. | Quantify the lowest noise level taken. Used for measuring background or ambient noise. |

For further information, [Pulsar Instruments](https://pulsarinstruments.com/news/what-are-ln-values-and-how-are-they-used/#:~:text=Ln%20values%20are%20statistical%20noise,timed%20measurement%20period%20(T).) has an article which explains statistical sound levels in greater depths.

---
## References
[1] M. Asselineau, *Building Acoustics*. Boca Raton, Florida: CRC Press, 2015.

[2] D. A. Bies, C. H. Hansen, and C. Q. Howard, *Engineering Noise Control*, 5th ed. Boca Raton, Florida: CRC Press, 2017.
