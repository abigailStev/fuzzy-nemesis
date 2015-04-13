Creates a power spectrum (psd, power spectral density) of X-ray timing data.
Intended to be used with event-mode RXTE data.

CONTENTS:

powerspec.py:
Makes a power spectrum for a light curve. Reads in a filtered event list from a
FITS or ASCII/txt/dat file, 'populates' each light curve segment, takes power 
spectrum of each segment, averages those power spectra over all segments of the
light curve, applies fractional rms^2 normalization (able to go into code to do
Leahy or absolute rms^2), computes sample frequency of averaged power spectrum, 
writes to a file.

rebin_powerspec.py:
Re-bins the power spectrum by frequency by a specified re-binning constant. 
Saves the re-binned power spectrum to a file, plots it logarithmically, and 
saves the plot.

plot_powerspec.py:
Linearly plots a power spectrum and saves the plot.

Note that 'tools.py' is in my git repo 'whizzy_scripts'.


This code comes with no guarantees.