# Metadata

## Dataset Title

Predictors of water uptake depth

## Authors

van Zyl, Michèle; Kretz, Lena; Sachsenmaier, Lena; Tölle, Max; Richter, Ronny; Weigelt, Alexandra; Wirth, Christian

## Version
v1.0.0

## Files

van_Zyl_et_al_2026_data_METADATA.csv

## Title

Mechanisms driving interspecific variation in tree water uptake depth

## Abstract

In this study, we investigated the drivers of interspecific variation in water uptake depth across 40 tree species (120 individuals) growing in the research arboretum (ARBOfun) in Großpösna near Leipzig, Germany. Stable oxygen isotopes and a two-end-member mixing model were used to estimate the proportion of shallow versus deep water uptake (fshallow and fdeep), while random forest models identified the climatic, morphological, and functional traits explaining variation in water uptake depth. fshallow was used as a response variable, and several variables were used as predictors: tree height, aridity and maximum temperature tolerance indices, drought tolerance index, sheltering index (shading potential), predicted rooting depth index, the mean soil moisture, growth response to drought and the position of a species on the LES (leaf economic spectrum) and P50 (xylem water potential at which a plant loses 50% of its hydraulic conductivity due to drought-induced embolism).

## Comments

Part of the dataset has already been published here:
https://doi.org/10.5281/zenodo.22117766
https://doi.org/10.5281/zenodo.21098915
https://doi.org/10.5281/zenodo.23081791

## Project

ARBOfun

## Geographic description

ARBOfun, Großpösna, Germany

- Latitude: 51°16′N
- Longitude: 12°30′E

## Data coverage

**Temporal description**

2024-2026

**Sampling design**

For the purpose of this study, 120 trees were sampled; these represent the Very Important Tree (VIT) selection. The aim of this selection was to identify 40 representative tree species

## Methods

### Field methods

Three 10 cm-long twigs were sampled from each of the 120 tree individuals (VITs) (40 species with 3 replicates each), from random positions in the canopy, facing different directions. Using a budding knife, the bark and cambium layer of the sampled twigs were removed up to the xylem layer.The sampling was done over two days in Summer (05 and 11 June, 2025).
On three separate days (11 April, 30 June and 04 August, 2025) during the growing season of 2025, soil cores were extracted (vibra-coring, with an Atlas Copco Cobra Pro hammer and 100 and 60 mm open corers) at three locations within the arboretum (Blocks A-C).
From each core, soil was collected from seven depths (10, 20, 50, 100, 150, 200, and 250 cm, with 0 cm representing the soil surface).

### Laboratory methods

Water from xylem and soil samples was extracted using a custom-built cryogenic vacuum distillation system at the Swiss Federal Institute for Forest, Snow and Landscape Research (WSL, Birmensdorf), following Diao et al. (2023), after which the extracted water was transferred into 1.5 mL gas-tight glass vial and refrigerated until further analysis.
δ18O measurements of water were done using a high-temperature reactor (TC/EA, Thermo Finnigan) with a tube-in-tube setup, coupled to a DeltaV isotope ratio mass spectrometer (IRMS, Thermo Fisher Scientific).

### Data analysis
To get a more accurate indicator of source water and to account for species getting water from more than just one source, a two-end member mixing model was performed. The conceptual model assumes that each tree’s δ18Otwig is a mixture of two soil water sources; shallow water and deep water (von.
The conceptual two-end member mixing model can be described mathematically with the function:
δ18Otwig = fshallow *δ18Oshallow + (1-fshallow)* δ18Odeep		(3)
where, 
fshallow = fraction of water from shallow soil, and,
1- fshallow = fraction from deep soil (fdeep)

For this study, shallow water was defined as source water found within the top 20 cm below ground (0 - 20 cm), whilst deep water refers to water below 20 cm underground (>20cm). This 20 cm boundary was selected based on the preliminary results. 
In addition, it was observed that the δ18O of the soil water (δ18Osoil) for the three sampling locations changed significantly over the three sampling dates in the shallow layers. Thus, only the δ18Osoil from the two summer sampling dates (30.06 and 04.08.2025) were used in the model, as they were closest to the dates of the twig sampling. 
Therefore, δ18Odeep was calculated as the mean δ18Osoil across the two sampling dates, across all three locations, for depths over 20 cm (50, 100, 150, 200, and 250 cm below ground), whilst δ18Oshallow refers to the mean δ18Osoil across the two sampling dates, across all three locations, for depths of 0 - 20 cm (10, 20 cm below ground). 

See van Zyl et al., 2026 for detailed description of analyses and how the other variables were collected/calculated.

Due to the data coming from various sources, there are several Na's (6% of data)- variables for which there is no data for the given species. 
Thus, in the paper, a gap- filling was also done using this data to create a more complete dataset. 
During the analyses of the isotope results, it was realised that one individual (Sor auc, block C), was sampled instead of Sor auc block D. This was because the individual included as a VIT changed in 2024. However, this individual was still included for analyses, even if it is no longer a VIT, in order to still have 3 replicates of the species. 
The names of the species are according to the World Checklist of Vascular Plants (WCVP)- because some of the names changed during the course of the experiment, the data refers to the old and new names

## Keywords

**General Descriptors**

-isotopes
-water uptake
-drought tolerance
-ARBOfun

**Organisms**

Plants; Trees

# DataStructure

Column Header	              Column Definition

species_former_code	        Previous species code/abbreviation, according to the old name
species_former_name	        Old species name, before the taxonomy was updated
species	                    Species name
species_code	              Species abbreviation
clade	                      Clade of the species
genus	                      Genus of the species
block	                      Block in which the tree is planted (A-E)
f_shallow	                  Fraction of shallow water uptake calculated with a two-end member mixing model
H_m	                        Height of the tree (Aboveground)
q10_aridity	                10th percentile of the aridity index (q10) used to characterize drought resistance for each species
q90_max_T	                  90th percentile of maximum temperature (q90) used as an indicator of upper heat tolerance
drought_tolerance_mean	    mean drought tolerance, extracted from Niinemets & Valladares (2006)
sheltering_index	          Sheltering index, as a measure of shading potential of the tree canopy (calculated from TLS scans)
pred_root_depth	            The predicted rooting depth
mean_soil_moisture	        Mean soil moisture for individual tree/sensor, across 6 days (3-5 June and 9-11 June 2025), where soil moisture calcualted as soil water content (SWC)
growth_response_mean	      Growth response to drought
PC1_score	                  Score of the first axis of a PCA from 7 leaf traits. This represents the species position on the LES axis from slow to fast strategies
P50	                        Xylem water potential at which a plant loses 50% of its hydraulic conductivity due to drought-induced embolism

## Contact

Michèle van Zyl | michele.ter_huurne@uni-leipzig.de

Feel free to get in touch with any questions on the data set.
