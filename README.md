# TKS System Properties
## General Data Files:
* File "tks_planet_properties-final.csv"
  * Includes all final planet properties from TKS sample (including both directly modeled transit parameters as well as derived planet properties)
  * Includes notes from M. MacDougall (i.e. comments on TTVs, variability, or other possible transit signals)
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

* Folder "tks_pipeline_outputs.zip"
  * Includes all pipeline outputs for each planet
  * All sub-folder names are labeled with "[TOI]_[TIC]"
    * Notation:
      * [SYSTEM_ID] = [TOI]_[TIC] (i.e. "T001272_TIC0417948359")
      * [PLANET_ID_NUMBER] (i.e. ".01" or ".02"; like in TOI-1255.01)
      * [PLANET_ID] = [TOI] + [PLANET_ID_NUMBER] (i.e. "1255.01")

## TOI-specific Data Files:
- [SYSTEM_ID]-[PLANET ID]-CORNER.png: corner plot of posteriors of period, t0, Rp/Rs, b, T14, ecc, omega, and {u1, u2}
- [SYSTEM_ID]-[PLANET ID]-FOLDED_FINAL.png: phase-folded lightcurve with final model fit and binned points
- [SYSTEM_ID]-[PLANET ID]-SUMMARY.csv: summary of 15th, 50th, and 85th percentiles of all modeled final transit parameters
- [SYSTEM_ID]-[PLANET ID_NUMBER]-TRACE.csv: samples of transit model fit (using *exoplanet*)
- [SYSTEM_ID]-[PLANET ID_NUMBER]-TRACE_FINAL.csv: final importance-sampled transit model posterior distribution data
- [SYSTEM_ID]-DATA.csv: input lightcurve photometry data
- [SYSTEM_ID]-FINAL_LC.png: full detrended lightcurve photometry with all transits marked

If TTVs were considered, then the following files are also available:
- [SYSTEM_ID]-[PLANET_ID]-TTVS_FINAL.csv: final transit times (both observed and calculated)
- [SYSTEM_ID]-[PLANET_ID]-TTVS_FINAL.png: plot of final TTVs

If TTVs were deemed significant, then the following files are also available:
- [SYSTEM_ID]-[PLANET_ID]-TTVS_SIGNAL_LS.png: plot of final TTVs with a sinusoidal curve fit to the data via a Lomb-Scargle periodogram
- [SYSTEM_ID]-[PLANET_ID]-TTVS_SIGNAL_L1.png: plot of final TTVs with a sinusoidal curve fit to the data via an l1 periodogram (see Hara et al. 2017)
