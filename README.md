
# Geometry
* AHDC and ATOF geometry services exist in COATJAVA and export to GEMC.
* Detector materials, target, support geometries should be checked. 

# Digitization 
* Sensitive volumes record GEANT hits, output in GEMC truth bank.
* ADC/TDC banks also output from GEMC.  Not final, pending real data(?).
  * How sophisticated is the GeV/ns -> ADC/TDC model?
  * How good does it need to be before investing more in reconstruction?
* Time-to-distance/DOCA (?) in GEMC in progress, based on Garfield. 


# Online
What exactly is required to confirm ALERT is recording good data?
## Existing tools
* slow controls
* mon12/hydra https://github.com/jeffersonlab/mon12
  * information is limited to ADC/TDC banks
  * visualize 1/2-D histograms
* ced
* online recon

# Calibration 
## ALERT Suite
## Alignment 
### Global 
### Internal 
