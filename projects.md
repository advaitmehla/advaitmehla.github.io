---
title: "Projects"
layout: splash
classes: 
    - landing
    - dark-theme
header:
  image: /assets/images/home.resized.jpeg
#   caption: "Yes, that is me"
permalink: /projects/
---

## My Projects

Here is a collection of some research projects that I have worked on over the years.

### Oxygen isotopic ratios of Hydrogen-deficient Carbon (HdC) stars ([Available on arXiv](https://arxiv.org/abs/2412.03664){:target="_blank" rel="noopener"}, [GitHub](https://github.com/advaitmehla/HdC-high-res))
Guides: Prof. Mansi Kasliwal (Caltech), Dr. Patrick Tisserand (Institut d'Astrophysique de Paris)

HdC stars are a rare class of supergiants that are hydrogen-deficient and carbon-rich. They are believed to be the merger products of a binary system consisting of CO and He white dwarfs, which leads to the formation of a star with anomalous abundances. HdC stars are further divided into two sub-classes -- the R Coronae Borealis (RCB) stars and dustless HdC (dLHdC) stars. While the former group is well known for its extreme variability characterized by sudden, random declines of upto 9 magnitudes caused by dust formation episodes, the latter shows no such variability. 

<p align="center">
  <img src="/assets/images/hdc.png" alt="fit" width="800px">
</p>

The nucleosynthesis processes that take place in the merged system are known to produce an overabundance of <sup>18</sup>O leading to <sup>16</sup>O/<sup>18</sup>O ratios that can be lower than 1, while the solar value is ~500. Moreover, it has been suggested that there exists a dichotomy in the <sup>16</sup>O/<sup>18</sup>O ratios of the two sub-classes, with dLHdC stars having ratios <1 and RCB stars having ratios >1. To accurately constrain these quantities, we must fit high resolution infrared spectra of these stars with synthetic spectra generated using model atmospheres, which has been the focus of my work. I developed a semi-automated routine ([Github](https://github.com/advaitmehla/TSFitPy)) to fit the spectra of these stars and robustly constrain their <sup>16</sup>O/<sup>18</sup>O ratios and other abundances. A sample fit obtained for one such star is shown above. We are currently in the process of compiling these results and preparing them for publication.

### Synthetic Photometry for Cryoscope
Guide: Prof. Mansi Kasliwal (Caltech)

Cryoscope is a new instrument being developed at Caltech that would enable time domain astronomy in the thermal infrared. The cryogenically cooled instrument is planned to be a meter-class telescope that will conduct a wide field survey in the K<sub>dark</sub> bandpass (2.25 -- 2.5 µm). It's location in the Antarctic provides a sky background that is 25 -- 40 times darker than temperate latitudes. The telescope's unique bandpass brings with it a host of challenges, including the lack of a standard star catalog in the K<sub>dark</sub> band, which necessitates the development of synthetic photometry techniques to calibrate the data, a task that I am working on.

<p align="center">
  <img src="/assets/images/cryo.png" alt="fit" width="500px">
</p>

This work involves utilizing existing photometric surveys to generate spectral energy distributions (SEDs) of stars that can be fitted to stellar atmospheric models, which can then be used to extrapolate the fluxes that we expect in the K<sub>dark</sub> band. This can then be vetted against near-infrared spectral libraries such as IRTF and X-Shooter to ensure that the synthetic photometry is accurate. The plot above shows an early result, indicating a mean error of less than 10% between the synthetic and observed fluxes when a combination of WISE and 2MASS data is used.

### Prospects of measuring Gamma-ray Burst Polarisation with the Daksha mission ([Published in JATIS](https://doi.org/10.1117/1.JATIS.9.4.048002){:target="_blank" rel="noopener"})
Guide: Prof. Varun Bhalerao (IIT Bombay)

The proposed Daksha mission comprises of a pair of highly sensitive space telescopes for detecting and characterising high-energy transients such as electromagnetic counterparts of gravitational wave events and gamma-ray bursts (GRBs). Along with spectral and timing analysis, Daksha can also undertake polarisation studies of these transients, providing data crucial for understanding the source geometry and physical processes governing high-energy emission. Each Daksha satellite will have 340 pixelated Cadmium Zinc Telluride (CZT) detectors arranged in a quasi-hemispherical configuration without any field-of-view collimation (open detectors). These CZT detectors are good polarimeters in the energy range 100 - 400 keV, and their ability to measure polarisation has been successfully demonstrated by the Cadmium Zinc Telluride Imager (CZTI) onboard AstroSat. Here we demonstrate the hard X-ray polarisation measurement capabilities of Daksha and estimate the polarisation measurement sensitivity (in terms of the Minimum Detectable Polarisation: MDP) using extensive simulations. We find that Daksha will have MDP of~30% for a fluence threshold of 1e−4 erg cm<sup>-2</sup> (in 10 - 1000 keV). We estimate that with this sensitivity, if GRBs are highly polarised, Daksha can measure the polarisation of about five GRBs per year.

### Implementing Nonlinear Control in a Classical Experiment to Reduce Measurement Noise ([Report](https://dcc.ligo.org/public/0188/T2300283/001/final.pdf){:target="_blank" rel="noopener"})
Guide: Prof. Rana Adhikari (Caltech)

Precise temperature control in the presence of noisy environments and heat loss through complex channels, involving conduction, convection, and radiation, presents a significant challenge. Traditional control methods, such as PID control, struggle to maintain a desired set-point due to system non-linearity and large disturbances caused by day-to-day ambient temperature fluctuations. The optimal tuning parameters also vary with external factors, further affecting performance.
In this project, we propose an adaptive control approach for nonlinear systems using neural networks trained via reinforcement learning. By introducing nonlinearity into the controller, we aim to address the limitations of traditional methods. The neural network-based controller leverages the entire state space, overcoming the challenge of non-separable and non-linear actuation functions where system parameters lack linear relationships.
Our approach offers several advantages for precise temperature regulation. Through reinforcement learning, the neural network controller learns to effectively respond to varying ambient conditions, adapt control signals, and dynamically adjust to disturbances. This adaptability eliminates the need for fixed tuning parameters, ensuring robust performance across different operating scenarios.
Extensive simulations are conducted to evaluate the proposed approach in realistic scenarios with diverse environmental conditions. The results demonstrate superior performance compared to traditional PID control methods. The neural network-based adaptive control exhibits enhanced set-point tracking accuracy and reduced sensitivity to low frequency (~1/day) fluctuations.
The significance of this work lies in its potential to advance temperature control in various nonlinear systems. By combining neural networks and reinforcement learning, our approach offers a practical solution for achieving precise control in the presence of disturbances. This work opens doors for the application of adaptive control in a wide range of fields where accurate control is essential in the face of complex dynamics and external fluctuations.

### Compton Imaging with the Daksha Mission ([Poster presented at ASI 2024](/assets/ASI_poster.pdf), [Thesis Report](/assets/BTP2.pdf))
Guide: Prof. Varun Bhalerao (IIT Bombay)

The proposed high-energy mission Daksha will continuously monitor the entire sky in the 1 - 1000 keV range with unprecedented sensitivity. The mission will contain an arrangement of 17 Medium Energy Packages consisting of a total of 340 Cadmium Zinc Telluride (CZT) detectors, sensitive in the 20-200 keV range. 13 of these are placed in a quasi-hemispherical arrangement, creating a dome - inside which are 4 High Energy Packages. These consist of Sodium Iodide (NaI) scintillators read by arrays of Silicon Photomultipliers (SiPMs) to cover the 100 keV - 1000 MeV energy range. Together, this geometry of detectors presents a unique opportunity to use Daksha as a Compton imager with all-sky sensitivity. This imaging method relies on the nature of Compton kinematics - where, given the incident and scattered photon energies, it is possible to localize rings of likely origin in the sky for each scattering event that is detected, known as ‘event circles’. These scattering events can be detected by isolating pairs of coincident events across detectors. With the detection of enough such pairs, it is possible to find the intersection of many event circles and hence successfully localize sources in the sky. Although the X-ray background dominates over most persistent sources for short exposures, integrating over timescales on the order of the five year mission lifetime could yield enough data to develop an all-sky map in the sub-MeV energy range, which would be the first of its kind. In this work, I explored results from extensive simulations of the Daksha mass model and detail the methodology used to reconstruct sources.
