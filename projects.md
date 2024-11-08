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

### Oxygen isotopic ratios of Hydrogen-deficient Carbon (HdC) stars
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


