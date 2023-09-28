# Alignment-of-HPLC-chromatograms

A_Libraries, is just all python libraries used and loaded.

00_Main, is the Main script is designed to run the four other scripts.

01_import, is the import of the files from the project.

02_wrangling, is the data wrangling performed for before feeding it to the models

03_Variable_and_model_selection, is all functions build to perform HPLC aligninment and classification.

The idea is to first perform data cleaning, and then select a window of interest, refering to retention time.

The data is then parced through a z-normalization, filtering, PCA, DTW-alignment algorithm and then clustered with k-means, soft clustering (fuzzy clustering).
The use of soft clustering is due to the need of dealing with multiple chromatograms within the same chromatogram being classed as the same peak.
