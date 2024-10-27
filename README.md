# Chemtronics Resource Page
----

[Direct Link](https://waterlevelshigh.github.io/CHEMTRONICS/)
### EPA Site Description
 >The 1,065-acre Chemtronics Superfund site is located in rural Swannanoa, North Carolina. The Superfund portion encompasses 535 acres of this property. The primary products manufactured on-Site were explosives, propellants, incapacitating agents, and a variety of specialty chemicals. Most of the manufacturing activities were discontinued by the late 1980s, and all manufacturing activities ceased in 1994.
#### Purpose of this page
Although site documents and data are readily available from the EPA sites, it can not be certain the data will exist in an unbroken state in the future. This page intends to collect all documents/data related to the Chemtronics superfund site including but not limited to:
- Five Year Reviews
- Archive images of operations
- Newspaper clippings
 - Administrative records/site decision
- Polygon/point features of Disposal Areas (DAs), Monitoring Wells (MWs), remediation structures, prior structures, suspected test pits.

#### "Doesn't the EPA keep track of this stuff?"
  Yes, but no publicly available data exists with site specific details including remediation/cleanup efforts, fill/disposal areas, and monitoring wells. The most recent Five Year Review (FYR) completed in August 2022 identifies features, however, this webmap intends to mimic the ESRI

_____

# Methods



---

# Changelog
#### [2023-02-14] - Local_Analysis
### Added
- High Resolution Orthoimagery of site from 2010
- Digital OrthoQuadrangle DOQ imagery from 1994, 95', 98'
- Digitized features
  - Former Buildings
  - Suspected pits
  - Ponds
  - Disposal areas
### Changed
- Changed the behavior and layout of the layer options offcanvas
  - Switched to bootstrap table format. Works well template at top.
  - Switched the color to a desaturated and 50% lighter shade of blue instead of mustard

#### [2023-02-13] - Page Created

### Added
- Index, readme, Refer to ../CHEMTRONICS_lOCAL for local analysis.
- assets dir: contains geojson of site features
- process_LiDAR.py to remove grid artifcats from lidar hillshades
  - DO NOT USE this on anything besides raw LiDAR 1M elevation models. The *elevation derivitaves* are hillshades derived from the LiDAR DEM already. Not sure why the artificats show up when analyzed locally but its annoying and process_LiDAR.py does remove most artifacts by aggregating points by a set factor, and creating a hillshade from that. RAW LiDAR datasets may need to be clipped by the site extent before detailed analysis

### Need
- Copy over the template for the web map from the SEBILCO site
- generate python to generate feature layers faster, i.e., function naming conventions and styling, refernces to properties, slider bars and dropdown menus. Opacity controls
- Polygon features for each previous structure, Disposal area
- point features for each monitoring well
Documents links stored locally, with attribution to epa site links.
