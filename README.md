# Geometry (COATJAVA+GEMC)
* AHDC and ATOF geometry services exist in COATJAVA and export to GEMC
* Detector materials, target, support geometries should be checked

# Digitization (GEMC)
* Sensitive volumes record GEANT hits, output in GEMC truth bank
* ADC/TDC banks also output from GEMC
  * Contents/schema not final, pending real data(?)
  * How sophisticated is the GeV/ns -> ADC/TDC model?
  * How good does it need to be before investing more in reconstruction?
* Time-to-distance/DOCA (?) in GEMC in progress, based on Garfield

# Reconstruction (COATJAVA)
## ATOF
## AHDC
* Simple clustering and track finding exists
* Is a simple, helical fit currently available?
* Kalmna filtering exists
  * parameters require tuning, e.g., uncertainties

# Online
What exactly is required to confirm ALERT is recording good data?
## Existing tools
* slow controls
* mon12/hydra https://github.com/jeffersonlab/mon12
  * limited to ADC/TDC banks
  * visualize 1/2-D histograms
* ced
  * 2D/3D visualization of ADC/TDC hits
  * offline it can draw tracks, clusters, etc. 
* online recon
  * runs CLARA services 
  * single events with extrememly long processing times cause issues

# Calibration 
## ALERT Suite
## Alignment 
### Global
### Internal
## Mock Calibration Challenge
