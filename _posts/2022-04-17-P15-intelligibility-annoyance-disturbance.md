---
title: "Intelligibility, Annoyance & Disturbance"
categories:
    - Blog
tags:
    - Acoustics
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
excerpt: "Brief introduction on the notion of intelligibility, annoyance and disturbance in acoustics."
---

# Inatelligibility (Quantitative)

> ***Intelligibility*** is the ability to understand speech under given conditions.

## Cases of Intelligibility

| Case | Desirable | Undesirable |
|----- |-----------|-------------|
| Purpose | To ensure speech is understandable | To ensure speech is not understandable & not disturbing |
| Example | conference hall, lecture theatre, etc | meeting room, bank, etc |

### Levels of Understanding in Intelligibility

| Level | Description |
|-------|-------------|
| Discretion | A situation where a sizable part of the speech signal is not understood by a listener, thus limiting the annoyance created by the speaker. This is the best one can achieve in an open space. |
| Privacy | A situation where speech is not understood under normal circumstances. This implies partitions (open space is ruled out). |
| Security | A situation where speech is not understood under any circumstance. |

## Factors that Control Intelligibility

| Factor | Description |
|--------|-------------|
| Signal-to-noise Ratio (SNR) | The louder the background noise, the smaller the speech signal will emerge above it and the more difficult it will be for the listener. |
| Reverberation Time | The longer the reverberation time, the more difficult it will be for the listener to catch the consonants and understand the spoken words. |
| Speaker & Listener Distance | The longer the distance, the more the acoustic attenuation, and thus the lower the received speech signal. |
| Visual Cues | The better the vision of the speaker by the listener, the better his understanding of the speech signal. |

## Assessment Methods for Intelligibility
The assessment of speech intelligibility can be performed through a list of words or sentencesbeing read by a normal speaker to a panel of normal-hearing listeners. Unfortunately, this method calls for a significant number of participants, which makes it costly and unpractical. More to the point, it is quite time-consuming and depending on the native language of the speaker and the listeners, scores can vary by as much as 20%.

Therefore, quantitative measurements were used more commonly nowadays which are listed as follows:

1. **%ALcons** (Percentage Articulation Loss of Consonants)
2. **STI** (Speech Transmission Index)
3. **STIPA** (Speech Transmission Index for Public Address)
4. **RASTI** (Rapid Speech Transmission Index)

To learn more on how intelligibility is measured in practice, I had found that NTi Audio's *XL2 Analyzer* which I had used before adopts [STIPA](https://www.nti-audio.com/Portals/0/data/en/NTi-Audio-AppNote-STIPA-Measurement.pdf) (also could be found [here](https://edwardloo.github.io/assets/pdf/NTi-Audio-AppNote-STIPA-Measurement.pdf)) for quick & portable measurements in generating STI report.

### %ALcons (Percentage Articulation Loss of Consonants)

> ***Percentage Articulation Loss of Consonants*** is an indication of the loss of speech intelligibility that occurs in difficult acoustic environments.

<img src = "https://user-images.githubusercontent.com/79191009/163700638-89bd88dc-c918-47e5-80d5-97b10458dac1.png" width = 700 height = 200>{: .align-center}

Where:
- ***RT***        = reverberation time [*s*]
- ***V***         = room volume [*m^3*]
- ***N_{tot}***   = total number of loudspeakers
- ***N_{dir}***   = number of loudspeaker contributing to direct (early) sound
- ***Q***         = directivity factor of source
- ***M***         = specialist modifier (assume M=1 for most situations)
- ***D_2***       = furthest distance from loudspeaker [*m*]

### Speech Transmission Index (STI)

> ***Speech Transmission Index*** (STI) is a quantitative measure of intelligibility whose value varies from 0 (Completely unintelligible) to 1 (perfect intelligibility).

![image](https://user-images.githubusercontent.com/79191009/163700849-c71efbad-48db-4a6b-b40e-c0d008ea7cc7.png){: .align-center}

### Common Scale in Interpreting Intelligibility

| STI | Remark | ALcons (*%*) |
|-----|--------|--------|
| 0 - 0.30 | Unacceptable | 100 - 33 |
| 0.30 - 0.45 | Poor | 33 - 15 |
| 0.45 - 0.60 | Fair | 15 - 7 |
| 0.60 - 0.75 | Good | 7 - 3 |
|0.75 - 1.00 | Excellent | 3 - 0 |

(Source: [sengpielaudio](http://www.sengpielaudio.com/calculator-ALcons-STI.htm))

| Space | STI |
|-------|-----|
| Theatre & Conference Room | 0.70 - 0.90 |
| Open-plan Office | 0 - 0.5 |

# Annoyance (Qualitative)

> ***Noise annoyance*** is defined as a feeling of resentment, displeasure, discomfort, dissatisfaction or offence which occurs when noise interferes with someone’s thoughts, feelings or activities.

- Since *annoyance* is a qualitative measure of feelings, huge number of surveys are usually necessary to apprehend the applicable criteria.
- In most cases, annoyance seldom results from one specific sound source, and often due to multiple factors including auditory, visual, & cultural factors.

# Disturbance (Qualitative)

> ***Noise disturbance*** is defined as any noise, sound or signal which unreasonably disturbs the comfort, peace, or repose of another person.

Lawyers had came up with a more detailed definition in clarifying the term "unreasonable" in the previous definition, which leads to the following definition:

> Noise disturbance is defined as any source of sound, which exceeds the noise limitations, permitted by the noise ordinance. Sources of sound shall include but not be limited to the following: amplified music, loudspeakers, radios, televisions, stereos, musical instruments, powered toys or models, swimming pools or spas, industrial machinery, manufacturing equipment, pole drivers, air compressors, paint sprayers, motors, pumps, blowers, air conditioners, cooling towers, ventilation fans, fork lifts, loaders, tractors, animals, concerts, mechanical equipment, human voices, electrical appliances, vacuum cleaners, powered equipment, chain saws, motor vehicles and attached equipment not operated on a street or highway, etc.

## Statutory Noise Nuisance
To apply noise control bylaws, a legislator eventually came up with a notion of statutory noise nuisance:

> A statutory noise nuisance is more than where the noise is a mere annoyance, but where it is viewed to have a significant impact on the health and well-being of those affected. Many factors are taken into account in determining if the noise amounts to a statutory nuisance, including:

| Factors | Remark |
|---------|--------|
| Location | Is the noise typical for the area? A cockerel crowing in the countryside would be more accepted than that in a quiet urban residential road. |
| Time of day | A statutory nuisance can exist at anytime of the day, however, the effects of noise late at night when most people are sleeping would be given greater weight than the same noise occurring during the day. |
| Frequency | How frequently is the plaintiff affected by the noise? Clearly noisy parties every weekend would be viewed differently to one held occasionally. |
| Duration | How long is the plaintiff disturbed? A dog barking at the postman or barking at cats occasionally passing by would be viewed differently to one barking most of the day. |
| Intensity | How loud is the noise? How intrusive? We all have different noise thresholds and tolerances. In determining nuisance the judgement would be how the noise would affect an ordinary individual, not someone who had a particular sensitivity to the noise complained of. |
| Number of people affected | A view will be taken on the number of people who are, or could be, affected by the noise. If only one person complains when the whole street could equally be affected, then there could be a challenge that the individual making the complaint could be unduly sensitive. |

A [survey](https://i-ince.org/files/publications/iince091.pdf) (also could be found [here](https://edwardloo.github.io/assets/pdf/I-INCE_2009.pdf)) on noise control legislation and regulations had been published by the International Institute of Noise Control Engineering (I-INCE) in 2009.

# Emergence, Exceedance, Intrusiveness
Although typical community noise control regulations will typically state noise limits, the use of simple sound level value, *LAeq* will not always correlate with the annoyance or to all situations. For instance:

> When the background noise level is high enough, there probably will not be much of a problem, as the intruding noise will probably be masked. But, when the background noise level is rather low, then the intruding noise will be perceived and identified.

To deal with this issue, standards and regulations use a quantity that describes the excess of particular noise over the background noise level as:

| Term | Country | Standard |
|------|---------|----------|
| Emergence | European | Final Draft International Standard (FDIS) ISO 1996 |
| Exceedance | U.S. | - |
| Intrusiveness | Australia | - |

---
# References
[1] M. Asselineau, *Building Acoustics*. Boca Raton, Florida: CRC Press, 2015.

[2] D. A. Bies, C. H. Hansen, and C. Q. Howard, *Engineering Noise Control*, 5th ed. Boca Raton, Florida: CRC Press, 2017.

[3] "*%Alcons*" Jun. 02, 2020. Accessed on Apr. 17, 2022. [Online]. Available: https://strutt.arup.com/help/Electroacoustics/ALCONS.htm

[4] "*STI*" Jun. 02, 2020. Accessed on Apr. 17, 2022. [Online]. Available: https://strutt.arup.com/help/Electroacoustics/STI.htm

[5] A. Sengpiel, *Intelligibility Conversion*, Accessed on Apr. 17, 2022. [Online]. Available: http://www.sengpielaudio.com/calculator-ALcons-STI.htm
