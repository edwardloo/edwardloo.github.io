---
title: "Impact Noise"
categories:
    - Blog
tags:
    - Acoustics
    - Building Acoustics
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
excerpt: "A review on impact noise"
---

## 1.0 Definition
> **Impact or "Impulse (loosely)" Noise** includes all forms of **high-intensity short-duration** sounds. The energy of an impact is usually **broadly distributed**, but spectral concentrations of energy can occur at various frequencies throughout the audible range.  

## 2.0 Impact versus Impulse Noise
### 2.1 Impact Noise
> **Impact Noise** (also **Reverberant B-wave**) is normally produced by non-explosive means (i.e., metal-to-metal impacts in industrial plant processes).

- Reverberant industrial environments where impact noises are usually heard causes the duration of impact noises to be longer than associated impulse noises.  

### 2.2 Impulse Noise
> **Impulse Noise** (also **Non-reverberant A-wave**) is defined as a short-duration sound characterized by a shock front pressure wave-form (i.e., instantaneous pressure rise) produced by sudden release of energy (i.e., explosives or gun blasts). 

- Impulse noises are typically generated in free-field environments where sound-reflecting surfaces that create reverberation are absent. 

![image](https://user-images.githubusercontent.com/79191009/179966250-f13429d8-828f-45fa-82bd-68a2d1e1bf43.png){:.align-center}

Figure 1: Schematic Representation of Two Basic Impulse Noise Pressure-Time Profiles (Source: [2]){: .text-center}
 
## 3.0 Measurement of Impact Noise
- Record the pressure-time history of the impact 
- Consider the response properties of the measuring device (rise time can be short as few microseconds and intensity high as 185 dB SPL) 
- Common impulse SLM have time constant of (30 - 40 ms) 
- Gunfire typically lasts for few hundred of microsecond (Common SLM underestimate impulse parameters) 
- Typical industrial impacts may last for 200 ms or more (Common SLM are suitable) 

## 4.0 Factors Affecting Impact Noise
### 4.1 Environmental Conditions
- Free field or reverberant enclosure 
- Angle of incidence 
- Extraneous noise and vibrations 

### 4.2 Noise Signatures
- *Industrial* - reverberant (ringing) and conforms to law of acoustics 
- *Blast (Shock) waves* - governs by physical principles that are different than the laws of acoustics 

## 5.0 Floor Impact Noise
- Measured in laboratory 
- Heavy slab with a framed 10 m^2 opening in the middle 
- Flanking transmission is negligible 
- Sole contribution of sound levels in receiving rooms from test floor radiation 
- The test floor is excited using impact (tapping) machine 
- One side note, impact noise on walls could be assessed similarly using a small impact machine (pendulous hammer) according to Swiss Engineers and Architects standards (SIA 181) 

The impact noise level, L_n is given by:

![image](https://user-images.githubusercontent.com/79191009/179967268-ec4fc320-3238-4858-ba2f-226923fd850f.png){:.align-center}

Where:
  - ***L_1*** = mean sound pressure level in reception room [dB]
  - ***S*** = area of floor specimen (10 m^2) [m^2]
  - ***A*** = equivalent absorptive area in the reception room [m^2]

### 5.1 Measurement Standards
- **ISO 140-6**: (100-3150 Hz, recently attempting to extend towards low-frequency region until 50 Hz) 
- **ASTM E492**: (125-4000 Hz) 

## 6.0 Impact Noise Transmission
Affected by: 
- Direct transmission through separating floor 
- Flanking transmission by all walls linked to the separating floor 
- Parasite transmission by leakages around a constructive element or duct/opening 

### 6.1 Measurement:
- Using an impact machine at the emission room 
- Measure the mean sound pressure level at the receiving room 
- Standardize the result by reverberation time (SPL measured in receiving room is sensitive to room absorption) 

Standardized impact noise level, ***L_{nT}*** is given by: 

![image](https://user-images.githubusercontent.com/79191009/179968167-74c65745-6b07-404a-b7bf-3fbf6b061221.png){:.align-center}

Where: 
- ***L_1***: mean sound pressure level in reception room [dB] 
- ***T***: reverberation time in receiving room [s] 
- ***T_0***: reference reverberation time (usually 0.5 s) [s] 

### 6.2 Measurement Standards
- **ISO 140-7** 
- **ISO 15712-2** 
- **ASTM 1007** (also account for ceiling underneath the floor) 

## 7.0 Rain Impact Noise
- Significant on light roof elements 
- Softer roof covering provide quieter rain impact noise 

### 7.1 Test Procedure Standard
- **ISO 140-18**

## 8.0 Single Number Rating
- **ASTM E989**: Impact Insulation Class (IIC) 
- **ISO717-2**: Normalized Weighted Impact Sound Index (***L_{nw}***) 

More reading between the two ratings [here](https://nrc-publications.canada.ca/eng/view/accepted/?id=b23a5bb8-d638-4bf6-b50f-0bba06348410).

## 9.0 Impact Noise Reduction by Floor Coverings
- **ISO 140-8**: Laboratory Measurements of the Reduction of Transmitted Impact Noise by Floor Coverings on a Heavyweight Standard Floor 
- **ASTM E2179**: Standards Test Method for Laboratory Measurement of the Effectiveness of Floor Coverings in Reducing Impact Sound Transmission Through Concrete Floors 

## 10.0 Walking Noise
- Walking noise is assessed by performing the measurement in the same room. 
- Measurement carried out using **EN 16205** standard (***L_{new}***) 


---
## References
[1] M. Asselineau, *Building Acoustics*. Boca Raton, Florida: CRC Press, 2015.

[2] D. A. Bies, C. H. Hansen, and C. Q. Howard, *Engineering Noise Control*, 5th ed. Boca Raton, Florida: CRC Press, 2017.

[3] M. J. Crocker,, *Handbook of Noise and Vibration Control*. Hoboken, New Jersey: John Wiley & Sons, Inc., 2007
