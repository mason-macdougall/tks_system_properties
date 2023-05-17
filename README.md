# TKS System Properties
## General Data Files:
* File `tks_planet_properties-final.csv`
  * Includes all final planet properties from TKS sample
    * Directly modeled transit parameters (w/ upper and lower uncertainties)
    * Derived planet properties
  * Includes notes from Mason MacDougall (i.e. comments on TTVs, variability, or other possible transit signals)
  * Includes a flag indicating if measured TTVs are significant or not
  * Final update as of May 1st, 2023
* File `tks_planet_properties-reference.csv`
  * Includes descriptions and units for all columns of TKS planet properties data

* File `tks_stellar_properties-final.csv`
  * Includes all final stellar properties from TKS sample
    * Final values modeled via *isocassify* (w/ upper and lower uncertainties)
    * Input values drawn from Gaia DR2 and 2MASS
    * Input values measured via *SpecMatch*
  * Final update as of 1 May 2023
* File `tks_stellar_properties-reference.csv`
  * Includes descriptions and units for all columns of TKS stellar properties data

* Folder `tks_pipeline_outputs/`
  * Includes all pipeline outputs for each planet
  * All sub-folder names are labeled with "[TOI]_[TIC]" (i.e. "T001272_TIC0417948359")
    * See `README.md` within `tks_pipeline_outputs/` folder for more details on TOI-specific files
