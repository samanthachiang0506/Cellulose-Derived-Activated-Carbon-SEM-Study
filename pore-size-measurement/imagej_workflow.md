# Pore Size Measurement Workflow (ImageJ)

This document summarizes the procedure used to measure pore sizes in 
cellulose-derived activated carbon using ImageJ. Two pore-size ranges were 
quantified: mesopores (~20 nm) and macropores (~2–3 μm). All measurements were 
performed on SEM images acquired from the SU7000 under low-voltage conditions.

---

## 1. Image Selection

Images were selected based on the following criteria:

- Clear contrast at pore boundaries  
- Minimal charging or contamination artifacts  
- Appropriate magnification for the pore scale being measured  
- Consistent working distance and accelerating voltage within each category  

Settings used:

### Mesopores
- 1.00 kV  
- 2.5 mm WD  
- 250,000× magnification  

### Macropores
- 0.20 kV  
- 2.5 mm WD  
- 2,500× magnification  

---

## 2. Calibration in ImageJ

Each image contained a scale bar. Calibration steps:

1. Open image in ImageJ  
2. Use **Straight Line Tool** to draw across the scale bar  
3. Select *Analyze → Set Scale*  
4. Enter the corresponding physical length (e.g., 200 nm or 2 μm)  
5. Confirm that “global scale” was not applied to avoid cross-image interference  

This ensured accurate pixel-to-micrometer/nanometer conversion.

---

## 3. Thresholding and Binary Conversion

To isolate pores from the carbon matrix:

1. Convert the image to 8-bit grayscale  
2. Apply *Image → Adjust → Threshold*  
3. Modify upper/lower bounds until pore edges were clearly isolated  
4. Convert to binary mask for measurement  

Thresholding was performed individually for each image to avoid bias.

---

## 4. Pore Measurement Procedure

With a binary image prepared:

1. Select *Analyze → Analyze Particles*  
2. Set appropriate size ranges:
   - Mesopores: 10–100 nm  
   - Macropores: 0.5–10 μm  
3. Enable:
   - Display results  
   - Show outlines  
   - Exclude edge objects  

4. Export data to `.csv` when needed  

This provided diameter values for each detected pore.

---

## 5. Results

### Mesopores
- Magnification: 250k×  
- Average measured pore diameter: **21.89 nm**  
- Features correspond to fine pore networks typical of activated carbon precursors  
- Resolution limits require careful threshold selection

### Macropores
- Magnification: 2.50k×  
- Average measured pore diameter: **2.493 μm**  
- These are structural voids formed during pyrolysis  
- Well resolved at low kV due to strong edge contrast

---

## 6. Notes and Considerations

- Mesopores cannot be fully resolved at mid- or high-voltage due to beam penetration depth  
- Low-voltage (0.20–1.00 kV) significantly improves edge detection  
- SU7000’s detector configuration provides stronger contrast for pore measurement  
- Threshold sensitivity is the primary source of error in nanoscale pore quantification  
- Consistent WD and coating thickness improve measurement accuracy  

---

## Summary

ImageJ enabled quantification of both nanometer-scale and micrometer-scale pores.  
Combined with low-voltage SEM imaging, this workflow produced reliable pore-size 
measurements across multiple length scales, demonstrating the multi-scale 
morphology of cellulose-derived activated carbon.

