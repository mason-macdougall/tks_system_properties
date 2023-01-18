# TKS System Properties
Notes: 
- File "tks_system_properties-[date].csv" includes all stellar and planetary properties from latest pipeline run
- Folder "planet_properties/" includes all pipeline outputs for each planet
- All folder names within "planet_properties/" are labeled with [TOI]_[TIC] (i.e. [SYSTEM_ID])

## Files include:
- [SYSTEM_ID]-[TOI ID]-CORNER_weighted.png: fully weighted corner plot of posteriors of period, t0, Rp/Rs, b, and T14
- [SYSTEM_ID]-[TOI ID]-ECC_OMEGA.png: 2D joint posterior distribution of ecc and omega
- [SYSTEM_ID]-[TOI ID]-TRANSIT_FIT.png: phase-folded lightcurve with final model fit and binned points
- [SYSTEM_ID]-[TOI ID]-WEIGHTED_SUMMARY.csv: summary of all final transit parameters
- [SYSTEM_ID]-DATA.csv: input lightcurve photometry data
- [SYSTEM_ID]-FULL_DETRENDED_LC.png: full detrended lightcurve photometry with all transits marked
