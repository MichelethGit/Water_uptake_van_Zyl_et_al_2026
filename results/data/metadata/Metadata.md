# Metadata

## Dataset Title

Leaf traits for 90 species from ARBOfun

## Authors

Kretz L., Nabel, N., von Sivers, L. ,Wirth C., Weigelt, A.

## Version

v1.0.0

## Files

- Kretz_et_al_2026_leaf_traits_ARBOfun_data.csv

## Title
ARBOfun_leaf_traits_DATA

## Abstract

This dataset contains leaf morphological and chemical trait measurements of 90 tree species collected in the ARBOfun arboretum. Measurements were conducted for 3–4 individuals per species in June 2023, with selected species remeasured in June 2025. Samples consisted of 10 angiosperm leaves or up to 40 gymnosperm needles per individual and were used to determine leaf area, fresh and dry mass, leaf thickness, toughness, and carbon and nitrogen concentrations.

## Comments

Part of the dataset has already been published here:

- DOI: 10.25829/idiv.3581-33ht28
- DOI: 10.25829/idiv.3603-afag37

## Project

ARBOfun

## Geographic description

ARBOfun, Großpösna, Germany

- Latitude: 51°16′N
- Longitude: 12°30′E

## Data coverage

**Temporal description**

single sample

**Sampling: 2023

19-June-2023 until 29-June-2023

**Sampling: 2025

20-June-2025 until 30-June-2025

**Sampling design**

In the ARBOfun we sampling 3 individuals per species and updated in 2025. The trees were planted in 2012 and 2014, thus they were growing there at least 9 years. See also https://www.lw.uni-leipzig.de/institut-fuer-biologie/abteilungen/spezielle-botanik-und-funktionelle-biodiversitaet/forschung/waldforschung#c987180 for it. The sampling design is also explained in Sanaei et al. 2025 DOI: 10.1038/s42003-025-07756-y

## Methods

### Field methods

At our site leaves were fully developed by mid June. We took samples of 10 leaves of angiosperms and up to 40 leaves of gymnosperms only mature and healthy sun leaves, that were south-facing at the middle of the upper third of the tree crown (very high trees were sampled in the middle of the middle third). We used ideally different branches.

### Laboratory methods

Toughness was measured with the resistance to punch test (Electric Test Stand TVM-N with dynamometer FH50) on 5 leaves, each one punch beside the mid vein in the middle of the leaf. Needles were punched in the middle. Thickness was measured with a caliper next to the spot of the punch test. Therefore the leaf was carefully cut with scissors. The 5 other leaves (for needles up to 40) were weighted with a fine scale weight. We separated leaves and petioles for weighting and scanning to be able to use the data separately. Petiole and leaves were weighted separately. Afterwards leaves and petioles were scanned with a flatbed Expression 11000XL scanner (Epson, UK), (1200 dpi, 24-bit colour). Afterwards the leaves and the petioles were dried in a drying oven at 70°C for 24–48 h. The dry weight was weighted afterwards. We treated all gymnosperms as leaves without petioles, thus they only have values for leaves, not for leaves with petioles. Only the leaves were analysed for C and N.

### Data analysis

Fresh mass was measured for leaves with petioles and for leaf laminas after petiole removal. Fresh petiole mass was calculated as the difference between these two measurements. For the dry weight and the size the leaves and the petioles were measured, while the values for leaves with petioles were calculated. Traits were calculated as SLA (specific leaf area) = A (leaf size) / Ml (dry weight); LMA (leaf mass per area) = Ml (dry weight) / A (leaf size); LDMC (leaf dry matter content) = Ml (dry weight) / M (fresh weight); Toughness and Thickness were calculated as mean of the 5 measurements; LTD (leaf tissue density) = Ml (dry weight) / V (leaf volume (A (leaf size) * T (thickness) * 0.1)). For two individuals of two different species (Picea glauca (block A) and Crataegus monogyna (block B)) LTD was calculated with thickness data from 2025 and weight and size from 2023 data.

## Keywords

**General Descriptors**

- Leaf traits
- experimental set-up
- ARBOfun

**Organisms**

Plants; Trees
|

# DataStructure

| Column Header            | Description                                                                                                                                                                             | Unit     | Method                                       |
|:-------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------|:---------------------------------------------|
| species                  | Species name                                                                                                                                                                            |          |                                              |
| species_author           | Authors abbreviation of the species                                                                                                                                                     |          |                                              |
| block_ID                 | ID of the block (A, B, C, D, E) the individuum is planted                                                                                                                               |          |                                              |
| clade                    | clade of the species: angiosperm/gymnosperm                                                                                                                                             |          |                                              |
| fr_weight_leaf_wp        | Fresh weight per leaf with petiole. Calculated as fresh weight leaves with petioles devided by number of replicates                                                                     | g        | weighted and devided by the number of leaves |
| fr_weight_leaf           | Fresh weight per leaf. Fresh weight leaves (without petioles) devided by number of replicates. All gymnosperms we definded without petiole.                                             | g        | weighted and devided by the number of leaves |
| fr_weight_petiole        | Fresh weight per petiole. Fresh weight of petioles devided by number of replicates.                                                                                                     | g        | weighted and devided by the number of leaves |
| dry_weight_leaf_wp       | Dry weight per leaf with the petiole. Calculates as dry weight leaves with petioles devided by number of replicates.                                                                    | g        | weighted and devided by the number of leaves |
| dry_weight_leaf          | Dry weight per leaf. Without petiole. Calculated as dry weight leaves without petioles devided by number of replicates. All gymnosperms we definded without petiole.                    | g        | weighted and devided by the number of leaves |
| dry_weight_petiole       | Dry weight per petiole. Dry weight petioles devided by number of replicates.                                                                                                            | g        | weighted and devided by the number of leaves |
| size_leaf_wp             | Mean size per leaf with the petiole. Calculated as mean size of a leaf plus mean size of a petiole.                                                                                     | cm²      | calculated                                   |
| size_leaf                | Mean size of a leaf. Scans analysed with imageJ, directly calculate size of all leaves devided by number of leaves. All gymnosperms we defined without petiole.                         | cm²      | Flatbed scanner (1200 dpi, 24-bit colour)    |
| size_petiole             | Mean size per petiole. Scans analysed with imageJ, directly calculate size of all petioles devided by number of petioles.                                                               | cm²      | Flatbed scanner (1200 dpi, 24-bit colour)    |
| thickness                | Thickness measure once per leaf with a caliper just next to the toughness measure (cut with scissors to get close to the toughness measurment). Repeated at 5 leaves and mean was taken | mm       | Caliper                                      |
| toughness                | Resistance to punch test once with the machine Electric Test Stand TVM-N with dynamometer FH50. Repeated at 5 leaves and mean was taken.                                                | N        | Resistance to punch                          |
| leaf_N                   | leaf nitrogen concentration of dry_weight_leaf                                                                                                                                          | %        | elemental analyzer                           |
| leaf_C                   | leaf carbon concentration of dry_weight_leaf                                                                                                                                            | %        | elemental analyzer                           |
| SLA_wp                   | Specific leaf area (SLA) of a leaf with petiole. Calculated as = A (size_leaf_wp) / Ml (dry_weight_leaf_wp).                                                                            | cm²/g    | calculated                                   |
| SLA                      | Specific leaf area (SLA) of a leaf. Calculated as = A (size_leaf) / Ml (dry_weight_leaf).                                                                                               | cm²/g    | calculated                                   |
| LMA_wp                   | Leaf mass per area (LMA) of a leaf with petiole. Calculated as = Ml (dry_weight_leaf_wp) / A (size_leaf_wp).                                                                            | g/cm²    | calculated                                   |
| LMA                      | Leaf mass per area (LMA) of a leaf. Calculated as = Ml (dry_weight_leaf) / A (size_leaf).                                                                                               | g/cm²    | calculated                                   |
| LDMC_wp                  | Leaf dry matter content (LDMC) af a leaf with petiole. Calculated as = Ml (dry weight_leaf_wp) / M (fresh weight_leaf_wp).                                                              | g/g      | calculated                                   |
| LDMC                     | Leaf dry matter content (LDMC) af a leaf. Calculated as = Ml (dry weight_leaf) / M (fresh weight_leaf).                                                                                 | g/g      | calculated                                   |
| volume_leaf_wp           | Volume of leaf with petiole. Calculated as = A (size_leaf_wp) * (T (thickness) * 0.1(converting unit)).                                                                                 | cm3      | calculated                                   |
| LTD_wp                   | Leaf tissue density with petiole. Calculated as Ml (dry_weight_leaf_wp) / V (volume_leaf_wp).                                                                                           | g / cm3  | calculated                                   |
| volume_leaf              | Volume of leaf. Calculated as = A (size_leaf) * (T (thickness) * 0.1(converting unit)).                                                                                                 | cm3      | calculated                                   |
| LTD                      | Leaf tissue density. Calculated as Ml (dry_weight_leaf) / V (volume_leaf).                                                                                                              | g / cm3  | calculated                                   |
| leaf_CN                  | leaf carbon concentration devided by leaf nitrogen concentration                                                                                                                        | unitless | calculated                                   |
| leaf_N_area              | calculated as leaf_N / SLA                                                                                                                                                              | g/cm2    | calculated                                   |
| sampling_year_morphology | Year the measurements of leaf morphology (fr_weight, dry_weight, size) were conducted.                                                                                                  | yr       |                                              |
| sampling_year_toughness  | Year the measurements of leaf thickness and toughness were conducted.                                                                                            | yr       |                                              |
| sampling_year_chemistry  | Year the measurements of leaf chemicals (leaf_N and leaf_C) were conducted.                                                                                                             | yr       |                                              |
| species_former_name      | former name of the species                                                                                                                                                              |          |                                              |


## Contact

Lena Kretz | lena.kretz@uni-leipzig.de

Feel free to get in touch with any questions on the data set.