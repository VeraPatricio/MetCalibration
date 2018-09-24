# Accuracy of strong line metallicity diagnostics at z~1

Paper: https://academic.oup.com/mnras/advance-article/doi/10.1093/mnras/sty2508/5097883?guestAccessKey=323a2804-2578-4294-918c-b37023ee110e

Each folder corresponds, roughly, to a section in the paper.

## Data

Takes all the data from several papers and writes it down to a single table (using astropy Tables).

The main output files are:
    
    data_corrected_MW_ext.dat: emission line fluxes corrected by the Milky Way extinction
    galaxy_properties.dat: mass, SFR, Te and others from the literature for this sample

## TeMethod

Here we calculate the electron temperature and correct for dust in ***Te_and_Dereddening.ipynb*** and then use this to calculate the direct metallicity in ***TeMetallicity.ipynb***

The main output files are:

    data_Te.dat: with the electron temperature and attenuation for each galaxy
    data_dered.dat: dust corrected emission line fluxes

## StrongLineMethods

Comparison of the metallicity derived using the direct method and the strong line calibrations.  
