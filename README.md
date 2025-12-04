# Cellulose-Derived-Activated-Carbon-SEM-Study

This repository documents the materials characterization workflow performed using 
the Hitachi SU3500 and SU7000 scanning electron microscopes (SEM). The objective 
of the project was to examine the microstructure and pore morphology of 
cellulose-derived activated carbon and to evaluate how key SEM parameters affect 
image clarity and contrast.

The work was completed as part of MSE1066 – Practical Aspects of Electron Microscopy 
at the University of Toronto.

---

## Project Objectives

- Characterize surface morphology and pore structure of activated carbon  
- Compare imaging performance between SU3500 and SU7000 instruments  
- Study the influence of accelerating voltage, working distance, aperture size, and detector modes  
- Document instrument limitations, artifacts, and troubleshooting steps  

---

## Sample Preparation

Detailed workflow is found in:  
`/sample-preparation/sample_prep_workflow.md`

Topics include:
- Carbon tape mounting  
- Sputter coating  
- Handling porous carbon samples  
- Considerations for minimizing charging and contamination  

---

## Imaging Parameters

Detailed notes are found in:  
`/imaging-parameters/`

Parameters included in the study:
- Accelerating voltage  
- Working distance  
- Aperture size  
- Detector selection (UD, MD, LD)  

---

## Results Overview

Results and images are located in the `/results/` directory.

### SU7000  
- Capable of stable imaging at low accelerating voltages  
- Clear pore boundaries and surface contrast  
- Effective multi-detector configuration  

### SU3500  
- Limited performance at very low kV  
- Usable at mid-range voltages  
- Lower surface contrast compared to SU7000  

A detailed comparison is summarized in `/results/comparison.md`.

---

## Pore Size Measurement

The pore-size measurement workflow using ImageJ is documented in:  
`/pore-size-measurement/imagej_workflow.md`

This includes thresholding steps, region selection, and measurement considerations 
for porous carbon structures.

---

## Troubleshooting and Artifacts

Relevant notes are located in `/troubleshooting/`.

Topics include:
- Contamination box artifact on SU7000  
- Beam-induced polymerization effects  
- Low-voltage imaging failure on SU3500  

---

## Summary of Technical Findings

- Low accelerating voltage provides useful surface detail but requires appropriate detector sensitivity.  
- Working distance has a significant effect on image resolution and depth-of-field.  
- Activated carbon exhibits multi-scale porosity, requiring careful image thresholding for measurement.  
- SU7000 provides stronger performance for surface-sensitive imaging compared to SU3500.  
- Sample preparation quality directly affects charging behavior and contrast.  

---

## Author

TsaiTung (Samantha) Chiang  
Materials Engineering – SEM/EDS, Microstructure Analysis
