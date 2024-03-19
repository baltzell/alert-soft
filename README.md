# Geometry (COATJAVA+GEMC)
* AHDC and ATOF geometry services exist in COATJAVA and export to GEMC
* Detector materials, target, support geometries should be checked

# Digitization (GEMC)
* ALERT sensitive volumes record GEANT hits and output in GEMC truth bank
* ADC/TDC banks also output from GEMC
  * With sector/layer/component/order
  * Contents/schema not final, pending real data(?)
* How sophisticated is the GeV/ns -> ADC/TDC model?
  * How good does it need to be before investing more in reconstruction?
* AHDC
  * Time-to-distance/DOCA(?) in GEMC in progress, based on Garfield
  * Conversion from GeV to ADC?
* ATOF
  * Some light propagation time and energy attenuation exists
  * A photo-electron efficiency exists
  * No conversion from GeV to ADC currently?

# Reconstruction (COATJAVA)
## ATOF
Nothing exists yet
1. Use geometry service to retrieve positions and dimensions of scintillator hits
1. Convert ADC/TDC to GeV/ns
## AHDC
* Simple clustering and track finding exists
* Kalmna filtering exists
  * parameters require tuning, e.g., uncertainties, currently copied from an RTPC
* Simple, helicial fit is currently not available (?)
* DOCA/Time-to-distance(?) in progress

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
