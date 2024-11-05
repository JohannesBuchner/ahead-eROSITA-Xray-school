Exercises
=====================

for Thursday of https://events.mpe.mpg.de/e/eRO-SDAS

Exercise 1: fitting a background model
--------------------------------------

Prerequisites:

* You need BXA and pyxspec installed
* You need a copy of the BXA folder https://github.com/JohannesBuchner/BXA/

Steps:

1. with the terminal, enter the "exercise1" folder
2. fit the background with the PCA background (see https://johannesbuchner.github.io/BXA/pca-background-models.html)::

    python3 path/to/your/BXA/autobackgroundmodel/fitbkg.py 020_BackgrSpec_00001.fits 020_SourceSpec_00001.fits

3. visually inspect the fit quality (pdf output files)
4. read the instructions of the script output.

Exercise 2: get galactic NH and redshift
----------------------------------------

Steps:

1. create a text file called 020_SourceSpec_00001.fits.z which contains the redshift of the source
2. create a text file called 020_SourceSpec_00001.fits.z which contains the redshift of the source look up the galactic NH of this source with https://www.swift.ac.uk/analysis/nhtot/ . The RA & Dec are stored in the FITS file header (use python/astropy or fitsheader or fv or topcat).
3. 

python3 /mnt/data/daten/PostDoc2/programming/BXA/gal.py 020_SourceSpec_00001.fits

