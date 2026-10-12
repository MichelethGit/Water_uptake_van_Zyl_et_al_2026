Metadata for:



Data set title: Stomata density and size of 12 conifer tree species



Authors: Sachsenmaier L., Franz S., Kahl A., Kretz L., Wirth C.



Version: v1.0.0







Files:

\- Sachsenmaier\_et\_al\_2026\_conifer\_stomata\_trait\_data.csv

\- Sachsenmaier\_et\_al\_2026\_Stomata\_micoscopic\_images.zip (contains ca. 1000 images in tif format)





Variables:



|variable|description|unit|data type|comment|
|-|-|-|-|-|
|species|scientific name of the tree species<br /><br />|none|character|full botanical names with authors: Abies alba Mill., Abies grandis (Douglas ex D.Don) Lindl., Cedrus deodara (Roxb. ex D.Don) G.Don, Larix decidua Mill., Picea abies (L.) H.Karst., Picea sitchensis (Bong.) Carrière, Pinus nigra J.F.Arnold, Pinus ponderosa Douglas ex C.Lawson, Pinus sylvestris L., Pseudotsuga menziesii (Mirb.) Franco, Taxus baccata L., Tsuga canadensis (L.) Carrière|
|tree\_id|unique identifier of the tree, with indication of species (abbreviation) and grid location in the ARBOfun research arboretum|none|character|e.g. Ace\_pla\_10\_6<br /><br />(3-4 trees per species were measured)|
|leaf\_id|identifier of the leaf <br />|none|integer|(3 leaves per tree were measured)|
|imprint\_position|identifier of the position on the epidermal imprint where the image was taken (1, 2, 3)|none|integer|for each imprint, we photographed three random positions (across needle length) at 100x magnification and measured one stomatal complex per position at 1000x magnification|
|GCL|length of the guard cell|µm|numeric||
|GCPW|width of the guard cell pair|µm|numeric||
|SCL|length of the stomatal complex|µm|numeric|frequently recorded as NA when boundaries of subsidiary cells are not clearly distinguishable in the images|
|SCW<br />|width of the stomatal complex|µm|numeric|frequently recorded as NA when boundaries of subsidiary cells are not clearly distinguishable in the images|
|PW|width of the pore aperture between the two guard cells|µm|numeric|reported for completeness, but to be interpreted with caution due to low measuremnt precision|
|SD\_ab|Stomatal density on the abaxial (lower) side of the needle, calculated as abaxial stomata count divided by field of view (FOV) area|N/mm²|numeric|For some needles that are round in cross-section, the distinction between abaxial and adaxial is ambiguous, so this value represents the stomatal density on the photographed side|
|SD\_ad|Stomatal density on the adaxial (upper) side of the needle, calculated as adaxial stomata count divided by FOV area.  |N/mm²|numeric|For needles without adaxial stomata, SD\_ad was set to 0. For needles with evenly distributed stomata around the needle, SD\_ad was set equal to SD\_ab|
|SD\_sbs|Stomatal density of the surface that actually bears stomata (stomata-bearing surface; sbs)|N/mm²|numeric|For needles without adaxial stomata: SD\_sbs = SD\_ab. For needles with stomata on both surfaces: SD\_sbs = average of SD\_ab and SD\_ad|
|SD\_fs|Stomatal density calculated across the entire needle surface (full surface; fs), including stomata-free areas|N/mm²|numeric|Needles with evenly distributed stomata: SD\_fs = SD\_ab; Needles with only abaxial stomata: SD\_fs = SD\_ab / 2; Needles with stomata on both sides: SD\_fs = average of SD\_ab and SD\_ad|
|image\_no\_100x|identifier of microscope image (100x magnification)corresponding to tiff file names (e.g. ARBOfun\_stomata\_001.tif)|none|integer|can be used to link trait measurements to image files|
|image\_no\_1000x|identifier of microscope image (1000x magnification)corresponding to tiff file names (e.g. ARBOfun\_stomata\_001.tif)|none|integer|can be used to link trait measurements to image files|





Methods summary:



This dataset contains stomatal density and size traits for 12 gymnosperm tree species sampled in the research arboretum ARBOfun (Germany). For each species, three mature, sun-exposed canopy trees were sampled during June–July 2025.



Leaf epidermal imprints were prepared using transparent nail varnish. Conifer needles were briefly immersed in hot water (80 °C) with detergent to remove epicuticular wax plugs prior to imprinting. Imprints were used for microscopic analysis of stomatal traits.



Microscopic images were taken at 100× and 1000× magnification using a Leica ICC50 W microscope camera. Stomatal density was determined from manual counts on 100× images and standardized by field-of-view area (1.1151284 mm²). Imaging covered the full needle width at three positions along each needle. Where needle width exceeded the microscope field of view, two adjacent images were taken and combined conceptually to ensure full coverage. In species with stomata on both adaxial and abaxial surfaces, additional images were recorded on both sides, resulting in up to four images per sampling position. If needle tissue did not fully occupy the field of view, non-tissue areas were excluded and density calculations were adjusted using the effective sampling area.



Data limitations:



Stomatal measurements may be affected by variation in imprint quality, particularly in senescent, dehydrated, or mechanically damaged leaf tissue. In some cases, incomplete or distorted imprints may limit the ability to resolve stomatal structures reliably. Although a short hot-water treatment was used to remove epicuticular waxes, overexposure can soften or degrade tissue and reduce imprint quality. Care was taken to standardize this step, but minor variation may remain. Imaging and measurements are sensitive to focal plane and image sharpness. Slight differences in focus can influence the apparent boundaries of stomatal structures, particularly in species with sunken or overlapping subsidiary cells. As a result, guard cell dimensions may be systematically underestimated in some species.

Pore width is associated with higher uncertainty due to limited optical resolution of the aperture in some images.



Contact:



Lena Sachsenmaier | lena.sachsenmaier.research@gmail.com



Feel free to get in touch with any questions on the data set.

