Metadata for: Stomatal density and size of 27 angiosperm tree species (research arboretum ARBOfun, Germany)



Data set title:



Authors: Kretz L., Sachsenmaier L., von Sivers L., Nabel N., Wirth C., Weigelt A.



Version: v1.0.0







File:

\- DATA\_stomatal\_density\_size\_angiosperm\_tree\_species\_ARBOfun.csv





Variables:



|variable|description|unit|data type|comment|
|-|-|-|-|-|
|species|scientific name of the tree species<br />|none|character|full botanical names with authors:<br />*Acer negundo* L., *Acer platanoides* L., *Acer pseudoplatanus* L., *Aesculus hippocastanum* L., *Alnus glutinosa* (L.) Gaertn., *Betula pendula* Roth, *Carpinus betulus* L., *Castanea sativa* Mill., *Cormus domestica* (L.) Spach, *Corylus colurna* L., *Fagus sylvatica* L., *Fraxinus excelsior* L., *Juglans regia* L., *Platanus x hispanica* Mill. ex Münchh., *Populus tremula* L., *Prunus avium* (L.) L., *Quercus pubescens* Willd., *Quercus robur* L., *Robinia pseudoacacia* L., *Salix caprea* L., *Salix fragilis* L., *Sorbus aucuparia* L., *Tilia cordata* Mill., *Tilia tomentosa* Moench, *Torminalis glaberrima* (Gand.) Sennikov \& Kurtto, *Ulmus laevis* Pall., *Ulmus minor* Mill.<br /><br />(please note: *Cormus domestica* was formerly known as *Sorbus domestica*, *Platanus x hispanica* as *Platanus x acerifolia*, and *Torminalis glaberrima* as *Sorbus torminalis*)|
|species\_code|abbreviation of the species name|none|character|e.g. Acer negundo --> Ace\_neg|
|block|block within the ARBOfun site (A, B, C, D, E); identifier of the tree|none|character|3 trees per species were measured|
|leaf\_id|identifier of the leaf|none|integer|3 leaves per tree were measured|
|imprint\_position|identifier of the randomly selected measurement position on the epidermal imprint (1, 2, 3)|none|integer|for each imprint, we selected three random positions|
|GCL|length of the guard cell|µm|numeric||
|GCPW|width of the guard cell pair|µm|numeric||
|PW|width of the pore aperture between the two guard cells|µm|numeric|reported for completeness; pore width measurements are subject to relatively low measurement precision|
|SD|Stomatal density on the abaxial (lower) side of the leaf|stomata mm⁻²|numeric|only *Salix fragilis* had stomata on the adaxial side as well (not measured)|





Methods summary:



This dataset contains stomatal density and size traits for 27 angiosperm tree species sampled in the ARBOfun research arboretum, Germany (51.2604° N, 12.4983° E).

See [https://doi.org/10.1111/plb.70024](https://doi.org/10.1111/plb.70024) for a detailed description of the research site.



For each species, 3 trees with each 3 mature, sun-exposed canopy leaves were sampled. Leaf material was collected in June 2023, with additional samples collected in June 2025 for individuals for which the original samples did not provide sufficiently reliable measurements.



Leaf epidermal imprints were prepared from the abaxial leaf surface using transparent nail varnish. Please note: The adaxial leaf surface was also inspected for stomata in all species. *Salix fragilis* was the only species in which stomata were observed on the adaxial surface, although at lower density than on the abaxial surface. Adaxial stomata were not measured; all stomatal traits reported in this dataset were measured on the abaxial surface.



Imprints were analysed using a standard light microscope (Leica DM300). Stomatal density was determined by manual counts at 400× magnification and expressed as the number of stomata per mm² (based on a field-of-view area of 0.159 mm²). Stomatal size traits (guard cell length, guard cell pair width, pore width) were measured manually at 1000× magnification using the ocular scale and are reported in µm.



Not all imprints provided sufficiently clear images for reliable measurement of stomatal size. This was particularly the case for species with sunken stomata (e.g. *Acer* spp.). Missing values (NA) for stomatal size traits therefore indicate that the respective imprint position did not allow reliable measurement but not the absence of stomata. Pore width is reported for completeness but should be interpreted with caution because of its relatively low measurement precision.



All measurement were performed by a single observer to ensure consistency.





Contact:



Lena Sachsenmaier | lena.sachsenmaier.research@gmail.com

Lena Kretz	  | lena.kretz@uni-leipzig.de



Feel free to get in touch with any questions on the data set.

