# RSO_populations
Data files to accompany 'Predicting RSO Populations Using a Neighbouring Orbits Technique' paper. CC-BY-4.0

[Predicting RSO Populations Using a Neighbouring Orbits Technique](https://academic.oup.com/rasti/advance-article/doi/10.1093/rasti/rzae034/7733820) Cooke et al. 2024.

## detectable_results_data
Data files used to generate Table 2 of the accompanying paper.

File names list the height and inclination of the default orbit, as well as the latitude from which simulated observations are carried out. Data is in csv format with 5+ columns:
  - Columns 1-4: Tested $h$ (h), $i$ (i), $\Omega$ (omega) and $\nu$ (nu) offset values (units of km, deg, deg, deg respectively)
  - Columns 5-8: Detectability result for a maximum relative velocity of 2.5, 5.0, 7.5 and 10.0 pix/s respectively (boolean)
  - Column 9: Sum of columns 5-8

For a subset of the data files the only tested velocity is 10.0 pix/s and the summation column is dropped.


## injection_recovery_data
Data files used to generate Figure 9 of the accompanying paper.

Files are separated based on the variable being tested:
  - $n$ (number of frames): 6, 8, 10, 12, 14 frames
  - $n_{\rm pix}$ (number of pixels): 25, 37, 50, 63, 75 pix
  - $t$ (exposure time): 250, 500, 750, 1000 ms

Data is in csv format with 3 columns:
  - Column 1: Injected target magnitude
  - Column 2: Injected target relative velocity (units of pix/s)
  - Column 3: Recovery result (boolean)
