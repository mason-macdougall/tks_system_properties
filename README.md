# TKS System Properties
Notes: 
- File "tks_planet_properties-final.csv" includes all final planet properties from TKS sample (including both directly modeled transit parameters as well as derived planet properties) -- final update as of 1 May 2023
- File "tks_planet_properties-reference.csv" includes descriptions and units for all columns of TKS planet properties data

- File "tks_stellar_properties-final.csv" includes all final stellar properties from TKS sample (including final values modeled via *isocassify*, input values drawn from Gaia DR2 and 2MASS, and input values measured via *SpecMatch*) -- final update as of 1 May 2023
- File "tks_stellar_properties-reference.csv" includes descriptions and units for all columns of TKS stellar properties data

- Folder "planet_properties/" includes all pipeline outputs for each planet
- All folder names within "planet_properties/" are labeled with [TOI]_[TIC] (i.e. [SYSTEM_ID])

## Files include:
- [SYSTEM_ID]-[TOI ID]-CORNER_weighted.png: fully weighted corner plot of posteriors of period, t0, Rp/Rs, b, and T14
- [SYSTEM_ID]-[TOI ID]-ECC_OMEGA.png: 2D joint posterior distribution of ecc and omega
- [SYSTEM_ID]-[TOI ID]-TRANSIT_FIT.png: phase-folded lightcurve with final model fit and binned points
- [SYSTEM_ID]-[TOI ID]-WEIGHTED_SUMMARY.csv: summary of all final transit parameters
- [SYSTEM_ID]-DATA.csv: input lightcurve photometry data
- [SYSTEM_ID]-FULL_DETRENDED_LC.png: full detrended lightcurve photometry with all transits marked
