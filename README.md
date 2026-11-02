# analysis_wbm_water_use
The following code is used to process, analyze, and interpret output from the Water Balance Model (WBM) to estimate how important glaciers are for downstream water uses; specifically evaluating the fraction of glacier-sourced water in rivers, the amount of glacier-sourced water that contributes to meet irrigation and domestic demands, and a first-order estimate of the equivalent number of people and amount of crops supported by glacier-sourced water.

The jupyter notebooks should be run in order of their numbers, which will generate all relevant figures, tables, and values used in an accompanying study. The default (i.e., if you do not change anything) is that the figures and tables will be produced in separate sub-directories. The figures are labeled "fig1_...", "fig2_...", which correspond to the figures and tables in the main text as well as "figs4_..." which correspond to figures in the extended data. Other figures where they are the same figure that are repeated multiple times for different emissions scenarios (e.g., Figure 2 and Extended Data Figures 1-3) are labeled in a manner that should be easy to follow (e.g., "maps-subregions-qmax_dif-wcities-ssp126.png").

The following provides a very brief overview of what each jupyter notebook does and includes:

- analysis_00_preprocessing_wbm_data.ipynb: pre-processes WBM data to ensure dimensions are named properly and values are correct thereby making raw files clean so that they are easier to understand and work with.

- analysis_01-people_processing.ipynb: analyzes and produces figures and tables concerning the number of people that are supported by glacier-sourced water.

- analysis_02-crop_processing.ipynb: analyzes and produces figures and tables concerning the amount of crop production that is supported by glacier-sourced water.

- analysis_03-global_figure.ipynb: formats various datasets to produce Figure 1 which shows temporal variations in runoff, glacier-sourced water, demands, and equivalent people and crops supported.

- analysis_04-map_figures.ipynb: formats various datasets to produce map figures to show spatial variations in various metrics of interest for different time periods, including Figure 2. Note that the user should specify the ssp according to 'ssp126', 'ssp245', 'ssp370', and 'ssp585' to produce maps for various emissions scenarios.

- analysis_05-RiverTransects-PerPixelPopAnalyses.ipynb: produces figures that show spatial variations in glacier-sourced water fractions as a function of various metrics including the distance from the glaciers.

- analysis_06_regional_figure_runoff_people_crops.ipynb: produces Figure S7 which shows temporal variations in glacier-sourced water, equivalent populations supported, and equivalent crop production supported.

- analysis_07_validation.ipynb: comparisons of our model output to previous studies that estimated the fraction of glacier-sourced water at a given location. These data were used to create Supplementary Table 1.
