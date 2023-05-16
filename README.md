# TKS System Properties
## General Data Files:
* File "tks_planet_properties-final.csv"
  * Includes all final planet properties from TKS sample (including both directly modeled transit parameters as well as derived planet properties)
  * Includes note from M. MacDougall
  * Includes a flag indicating if measured TTVs are significant or not
  * Final update as of May 1st, 2023
* File "tks_planet_properties-reference.csv
  * Includes descriptions and units for all columns of TKS planet properties data

* File "tks_stellar_properties-final.csv"
  * Includes all final stellar properties from TKS sample
    * Final values modeled via *isocassify*
    * Input values drawn from Gaia DR2 and 2MASS
    * Input values measured via *SpecMatch*
  * Final update as of 1 May 2023
* File "tks_stellar_properties-reference.csv"
  * Includes descriptions and units for all columns of TKS stellar properties data

* Folder "planet_properties/" includes all pipeline outputs for each planet
- All folder names within "planet_properties/" are labeled with [TOI]_[TIC] (i.e. [SYSTEM_ID])

## TOI-specific Data Files:
- [SYSTEM_ID]-[TOI ID]-CORNER_weighted.png: fully weighted corner plot of posteriors of period, t0, Rp/Rs, b, and T14
- [SYSTEM_ID]-[TOI ID]-ECC_OMEGA.png: 2D joint posterior distribution of ecc and omega
- [SYSTEM_ID]-[TOI ID]-TRANSIT_FIT.png: phase-folded lightcurve with final model fit and binned points
- [SYSTEM_ID]-[TOI ID]-WEIGHTED_SUMMARY.csv: summary of all final transit parameters
- [SYSTEM_ID]-DATA.csv: input lightcurve photometry data
- [SYSTEM_ID]-FULL_DETRENDED_LC.png: full detrended lightcurve photometry with all transits marked
