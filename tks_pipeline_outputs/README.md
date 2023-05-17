## TKS Pipeline Output Data Files (TOI-specific):
General TOI system outputs:
- `[SYSTEM_ID]-DATA.csv.zip` --> compressed input lightcurve photometry data ("X" = time, "Y" = flux, "YERR" = flux error, "TREND" = Gaussian Process variability trend, "OUTLIERS" = mask to exclude significant outliers, "MASK" = mask to only include transits)
- `[SYSTEM_ID]-FINAL_LC.png` --> full detrended lightcurve photometry with all transits marked

Planet-specific outputs:
- `[SYSTEM_ID]-[PLANET ID]-CORNER.png` --> corner plot of posteriors of period, t0, Rp/Rs, b, T14, ecc, omega, and {u1, u2}
- `[SYSTEM_ID]-[PLANET ID]-FOLDED_FINAL.png` --> phase-folded lightcurve with final model fit and binned points
- `[SYSTEM_ID]-[PLANET ID]-SUMMARY.csv` --> summary of 15th, 50th, and 85th percentiles of all modeled final transit parameters
- `[SYSTEM_ID]-[PLANET ID_NUMBER]-TRACE.csv` --> samples of transit model fit (using *exoplanet*)
- `[SYSTEM_ID]-[PLANET ID_NUMBER]-TRACE_FINAL.csv` --> final importance-sampled transit model posterior distribution data
If TTVs were considered, then the following files are also available:
- `[SYSTEM_ID]-[PLANET_ID]-TTVS_FINAL.csv` --> final transit times (both observed and calculated)
- `[SYSTEM_ID]-[PLANET_ID]-TTVS_FINAL.png` --> plot of final TTVs
If TTVs were deemed significant, then the following files are also available:
- `[SYSTEM_ID]-[PLANET_ID]-TTVS_SIGNAL_LS.png` --> plot of final TTVs with a sinusoidal curve fit to the data via a Lomb-Scargle periodogram
- `[SYSTEM_ID]-[PLANET_ID]-TTVS_SIGNAL_L1.png` --> plot of final TTVs with a sinusoidal curve fit to the data via an l1 periodogram (see Hara et al. 2017)


Notation:
- [SYSTEM_ID] = [TOI]_[TIC] (i.e. "T001272_TIC0417948359")
- [PLANET_ID_NUMBER] (i.e. ".01" or ".02"; like in TOI-1255.01)
- [PLANET_ID] = [TOI] + [PLANET_ID_NUMBER] (i.e. "1255.01")


