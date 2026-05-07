Links:
Main paper: Iverson, L.R.; et al 2019. https://doi.org/10.3390/f10110989

Visualizations:
https://stellarore.github.io/USFS-tree-atlas/

https://public.tableau.com/app/profile/chris.b4242/viz/shared/284YMCTTW

https://public.tableau.com/app/profile/chris.b4242/viz/shared/DJTK73D35

Tree Atlas:
https://www.fs.usda.gov/nrs/atlas/combined/resources/summaries/ecomap/

https://www.fs.usda.gov/nrs/atlas/tree/

https://www.fs.usda.gov/nrs/atlas/tree/v4/modals/info.php#top

Visualization Notes:
Paper background:
Trees are a keystone species in many ecosystems. Climate change threatens them and all species that rely on them for food and habitat.  In Iverson, L.R.; et al (2019), the authors use Forestry Inventory Assessment data from the US Forestry Service to identify current habitat conditions for 135 tree species across the eastern US. They then predict future climate conditions (at 2100) under RCP4.5 and RCP8.5 (IPCC5 2013), and identify ranges where these species will likely maintain, expand, or lose population. This was intended as a guide for local forest managers to choose species to propagate and protect in their regions that have the best chances at surviving a changing climate. It was limited to the east of 100degW due to limitations in funding, data, and knowledge on western ecosystems. However, efforts are underway to expand the scope of our models to the western United States as well as Canada.

They have released their data as a series of excel sheets, each describing a region with its tree species.  Each species has a variety of data, notably FIAsum (FIA area-weighted importance value), FIAiv (FIA average species wide importance value), and SSO (species selection option). The importance value is calculated from the number of trees within a zone and their basal areas (trunk cross sectional area). Importance Values(X) = (50 * basal area(X) / basal area(all species)) + (50 * number of stems(X) / number of stems(all species)), where X is a single species. SSO was determined by a tree’s current abundance, species’s adaptability and how the climate is predicted to change.

If a species has a SSO = 0,1 or 2, it is currently found within the zone.  If SSO =0, according to the climate and habitat modeling, the species does not have a good chance at surviving in the future. 

Creating the index
Using these SSO values I have calculated an index for each zone to evaluate how well the current forest composition can handle impending climate change where:

Index = sum of trees ([Importance Value] * [SSO (0 or 1)]) / ( sum of trees ([Importance Value])) - 1.00

where Importance Value can be FIAsum or FIAiv. If a zone has species with all SSO = 1 or 2 (all species survive), the yellow and green terms will cancel to 1.00, leaving an index = 0.  If all species have SSO = 0 (all species struggle/die-off), the first term will be zero, leaving an index = -1.00.  The greater a single species’s Importance Value, the greater the loss for the ecosystem will be if SSO = 0, and the index will be closer to -1.00.  

Looking at the maps overall, the relative index values among the zones look comparable, whether using FIAsum or FIAiv. Northern MN and southern TX show better indexes under FIAiv. 
FIAsum _ FIAiv 

Forest Inventory Assessment (FIA) / National Forest Inventory (NFI)
The FIA program collects and reports information about the nation's forest lands, and beginning in 1999, implemented annual inventories completed over a 5‐ to 7‐year cycle (O'Connell et al., 2017). However, due to insufficient funding, cycles for some states were extended. Sampling of forest conditions and individual trees ≥5.0 inches in DBH is performed on four 24‐foot radius sub- plots (O'Connell et al., 2017).

The Nationwide Forest Inventory (NFI) consists of a probabilistic sample of permanent plots installed across all forested lands (or lands capable of being forested) in the US. The sample design consists of one field plot for every 6,000 acres (24 km2) of forest. Field crews collect information on forest type, site attributes such as ownership and terrain, tree species, tree size, and overall tree condition. On a subset of sample plots, FIA measures a broader suite of attributes including understory vegetation, down woody material, and soil information. Soil samples are sent to a laboratory for chemical analysis. Each plot is measured every 5-10 years, depending on the state the plot falls within. Each step of the inventory process, from field preparation to publication of data and reports, goes through quality assurance procedures to ensure high data quality. Remote sensing data are combined with the plot data, using an analysis method known as post-stratified estimation, which produces more precise estimates of forest conditions than using the plot data alone.


Possible visualization grouping zones:
By state
EcoMap 2007
https://databasin.org/datasets/662c543156c14313b87d9b99b7a78221/
Ecological units are mapped based on associations of biotic and environmental factors that directly affect or indirectly express energy, moisture, and nutrient gradients which regulate the structure and function of ecosystems. These factors include climate, physiography, water, soils, air, hydrology, and potential natural communities.



Watersheds:
1x1 degree grid (~100km x ~100km)
National Climate Assessment regions:

Ecoregional Vulnerability Assessments (EVAS)



2010 Census Urban zones


