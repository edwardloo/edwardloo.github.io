---
title: "Sound Insulation"
categories:
    - Blog
tags:
    - Acoustics
    - Building Acoustics
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
excerpt: "A comprehensive review on acoustic or sound insulation."
---

## Sound Insulation
Sound insulation is commonly quantified using the ***Sound Reduction Index (SRI), R***.

### Sound Reduction Index, *R*

![image](https://user-images.githubusercontent.com/79191009/167237595-4667a1e3-4e60-4462-b86c-9b31cdf95664.png){: .align-center}

Where:
  - ***R***     = sound reduction index 
  - ***L_1***   = mean sound pressure level in emission room [*dB*]
  - ***L_2***   = mean sound pressure level in the reception room [*dB*]
  - ***S***     = area of the floor or wall specimen under test [*m^2*]
  - ***A***     = equivalent absorptive area in the reception room [*m^2*]

#### Laboratory Measurement of SRI
  1. Usually conducted on a wall or floor speciment in laboratory
  2. The laboratory features heavy slabs and walls with a framed 10 *m^2* opening in the middle
  3. The envelop of the measurement room is separated by expansion joint (negligible flanking transmission)
  4. The previous condition ensures that the contribution to sound levels measured in receiving room is solely from radiation of specimen under test
  5. The specimen is excited using a diffuse sound field (generated with loudspeakers durected tiwards the corners opposite to specimen under test) in the emission room
  6. The mean sound pressure level is measured in both the emission and receiving room

#### Standards for SRI Laboratory Measurements

| Standard | Description |
|----------|-------------|
| ISO 140-3 | 100-3150 *Hz* |
| ASTM E90 | 125-4000 *Hz* |
| EN/ISO 10140-3 | Attempt to extend the range in low-frequency region down to 50 Hz third octave band |

**Note:** It is advised to perform the specimen (wall, roof or floor sample) using dimensions as close as possible to the dimensions used in project. Using smaller dimension tends to **overestimate** the performance  **low-frequency range**.

#### Doubling Sound Insulation
The effect of a doubling is characterized by the ***sound reduction improvement index, ΔR*** which is defined as:

![image](https://user-images.githubusercontent.com/79191009/167238377-25ee52d5-7efd-4dbc-bdd7-ed6a96936857.png){: .align-center}

Where:
  - ***ΔR***                      = sound improvemnt index
  - ***R_{wall with doubling}***  = measurement of the sound reduction index of that wall with its doubling
  - ***R_{wall alone}***          = measurement of the sound reduction index of the main wall

**Note:**
  - the lighter the wall, the larger the ***ΔR*** value
  - the more porous the wall, the larger the ***ΔR*** value
  - negative value for ***ΔR*** (i.e., -4 to -7 *dB*) is possible (e.g., plasterboard on polystyrene doubling glued on a brick wall)
  - make sure that the doubling under consideration will not hamper the overall sound reduction performance of the wall construction 

### Other Factors Affecting Sound Insulation
#### Flanking & Parasite Transmission
Direction transmission that is characterized by sound reduction index, *R* is not the sole factor that affects the sound insulation between 2 spaces. ***Flanking transmission*** is the transmission of sound by walls or floors linked to the separating element. Whereas, ***parasite transmission*** is the sound leakage around a contructive element or through a duct or opening. Figure 1 below illustrates few transmission paths between 2 spaces.

![image](https://user-images.githubusercontent.com/79191009/167239072-c6bee032-05e7-42e9-91c9-9edec3839ec9.png){: .align-center}

Figure 1: Direct and Flanking Transmission between Rooms (Source: [1])
{: .text-center}

To quantify the overall contribution of all the factors mentioned, the sound insulation between rooms is also commonly characterized using the sound level difference, ***D***:

![image](https://user-images.githubusercontent.com/79191009/167239183-c9f3d33b-fb76-466a-a275-dd4dabfeb321.png){: .align-center}

However, the sound insulation value is dependent on the amount of acoustic absorption inside the receiving room. Therefore, the usual rule is to standardize the result by the reverberation time. Which gives the ***standardized sound insulation, DnT***:

![image](https://user-images.githubusercontent.com/79191009/167239269-a230fda5-b643-4ee9-85d8-298d0b76e8f0.png){: .align-center}

Where:
  - ***D***       = sound level difference
  - ***D_{nT}***  = standardized sound insulation
  - ***L_1***     = mean sound pressure level in the emission room [*dB*]
  - ***L_2***     = mean sound pressure level in the reception room [*dB*]
  - ***T***       = reverberation time in the reception room [*s*]
  - ***T_0***     = reference reverberation time (usually 0.5 s) [*s*]

| Standard | Description |
|----------|-------------|
| ISO 140-4 | 100-3150 *Hz* |
| ASTM 336 | 125-4000 *Hz* or 100-5000 *Hz* (France) |
| EN/ISO 16283-1 | Attempt to extend the range in low-frequency region down to 50 Hz third octave band |

The effect on the sound field of a slightly leaky room is shown in Figure 2 below.

![image](https://user-images.githubusercontent.com/79191009/167239523-5d432b5e-3d25-4d93-ac7d-590120d1ca36.png){: .align-center}

Figure 2: Example of Sound Intensity Contours Benhind a Window, Either Closed (Left) or Slightly Opened (Right) (Source: [1])
{: .text-center}

### Single Number Rating
To speed up the rating of specimens, experts usually rely on single number rating. It is an obvious simplification compared to the usual 6 octave bands (125-4000 *Hz*). ASTM had came up with the **Sound Transmission Class (STC)** which features a sliding contour. The contour runs 9 *dB* per octave from 125 to 500 *Hz*, 3 *dB* per octave from 500 to 1250 *Hz* and stays flat from 1250 to 4000 *Hz*. 

To determine the *STC* value, one glides the contour over the sound reduction or sound insulation curved measured until the sum of negative deviations is no greater than 32 *dB* and the maximum negative deviation is 8 *dB*. Whereas ISO uses the *R_w* or *D_w* system, which is similar but the frequency range is 100 to 3150 *Hz*. To cope with low frequencies down to 50 *Hz*, ISO has extended its *R_w* contour in standard ***ISO 16717-1***.

### Computing Sound Reduction Index
The most fundamental and crudest model is the mass law.

![image](https://user-images.githubusercontent.com/79191009/167240075-0cfa47d4-a716-4074-98f7-d11f31d8bd29.png){: .align-center}

Where:
  - ***R*** = sound reduction index for a single wall
  - ***m*** = mass per unit area of the wall or floor [*kg/m^2*]
  - ***f*** = frequency [*Hz*]

### Computing Sound Insulation
There are a few computer programs available to try to compute the sound insulation between rooms. Such programs rely on the knowledge of the sound reduction index of the various walls, as well as their coupling parameters, and operate according to **ISO 12354**. Most of the time they come with a rather significant database.

### Noise Radiated by a Construction
The noise radiated by a building will depend on the sound reduction index of each envelop componenet as well as respective area.

![image](https://user-images.githubusercontent.com/79191009/167240273-7eff3d36-949e-4dda-ac51-7e374d498750.png){: .align-center}

Where:
  - ***L_w*** = sound power level radiated by a component
  - ***L_p*** = sound pressure level inside the building
  - ***S*** = surface area of component tested
  - ***R*** = sound reduction index of component

---
## References
[1] M. Asselineau, *Building Acoustics*. Boca Raton, Florida: CRC Press, 2015.

[2] D. A. Bies, C. H. Hansen, and C. Q. Howard, *Engineering Noise Control*, 5th ed. Boca Raton, Florida: CRC Press, 2017.
