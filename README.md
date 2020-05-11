﻿# Collection of custom scripts

## Custom Scripts Repository

This repository contains a collection of custom scripts for [Sentinel Hub](https://www.sentinel-hub.com/), which can be fed to the services via the URL.

Scripts are organised by sensors supported on Sentinel Hub:
  - [Sentinel-1](#sentinel-1)
  - [Sentinel-2](#sentinel-2)
  - [Sentinel-3](#sentinel-3)
  - [Sentinel-5P](#sentinel-5P)
  - [Landsat 5 and 7](#landsat-57)
  - [Landsat-8](#landsat-8)
  - [MODIS](#modis)
  - [PlanetScope](#planet_scope)
  - [Airbus Pleiades](#airbus_pleiades)

You are invited to publish your own scripts - see [howto](#howto).

## Relevant reading
* [Multi-temporal Processing](https://medium.com/sentinel-hub/multi-temporal-processing-6a80e5c84188) 
* [Color Correction with JavaScript](https://medium.com/sentinel-hub/color-correction-with-javascript-d721e12a919) (by Miha Kadunc)
* [Multi-year time series of multi-spectral data viewed and analyzed in Sentinel Hub](https://medium.com/sentinel-hub/multi-year-time-series-of-multi-spectral-data-viewed-and-analyzed-in-sentinel-hub-5628ec4fad9c) (by Grega Milcinski)
* [The Use of Satellite Imagery in Crisis Management after Flooding](https://medium.com/sentinel-hub/the-use-of-satellite-imagery-in-crisis-management-after-flooding-382be517224f) 
* [How to Create Cloudless Mosaics](https://medium.com/sentinel-hub/how-to-create-cloudless-mosaics-37910a2b8fa8) 
* [Educational Role of EO Browser and New Features](https://medium.com/sentinel-hub/educational-role-of-eo-browser-and-new-features-5bc6ea8d8143) (by Sabina Dolenc)
* [Environmental Monitoring of Conflicts using Sentinel-2 data](https://medium.com/sentinel-hub/environmental-monitoring-of-conflicts-using-sentinel-2-61f07d76e27b) (by Wim Zwijnenburg)
* [Why Newsrooms need People with Expertise in Remote Sensing](https://medium.com/sentinel-hub/why-newsrooms-need-people-with-expertise-in-remote-sensing-a8e83cedda0a) (by Pierre Markuse)
* [Active Volcanoes as Seen from Space](https://medium.com/sentinel-hub/active-volcanoes-as-seen-from-space-9d1de0133733) (by Sabina Dolenc)
* [Get Creative and Solve a Remote Sensing Problem at Home from your PC and Win!](https://medium.com/sentinel-hub/get-creative-and-solve-a-remote-sensing-problem-at-home-from-your-pc-and-win-9353938d5fff) (by Grega Milcinski)
* [Measuring Air Pollution from Space](https://medium.com/sentinel-hub/measuring-air-pollution-from-space-7492f5dad7bc) (by Sabina Dolenc)
* [Mapping deforestation with Sentinel Hub](https://medium.com/sentinel-hub/mapping-deforestation-from-sentinel-hub-de6aae67f817) (by Nicolas Karasiak)
* [Why join the next Sentinel Hub Custom Script Contest](https://medium.com/sentinel-hub/why-to-join-the-next-sentinel-hub-custom-script-contest-f3adb6c8e92c) (by Sabina Dolenc)
* [Learning Custom Scripts to make Useful and Beautiful Satellite images](https://medium.com/sentinel-hub/create-useful-and-beautiful-satellite-images-with-custom-scripts-8ef0e6a474c6) (by Monja Šebela)
* [It’s a faaaake… — Or not?](https://medium.com/sentinel-hub/its-a-faaaake-or-not-bace4f0c01ec) (by Pierre Markuse)
* [Custom scripts: faster, cheaper, better!](https://medium.com/sentinel-hub/custom-scripts-faster-cheaper-better-83f73894658a) (by Monja Šebela)
* [Water Quality Information for Everyone](https://medium.com/sentinel-hub/water-quality-information-for-everyone-a81faab8ff5e) 
* [New Themes, Multi-Temporal Scripting and Other Improvements in EO Browser](https://medium.com/sentinel-hub/new-themes-multi-temporal-scripting-and-other-improvements-in-eo-browser-725267d09f2f) (by Monja Šebela)

## <a name="sentinel-1"></a>Sentinel-1
The Sentinel-1 imagery is provided by two polar-orbiting satellites, operating day and night performing C-band synthetic aperture radar imaging, enabling them to acquire imagery regardless of the weather. Main applications are for monitoring sea ice, oil spills, marine winds, waves & currents, land-use change, land deformation among others, and to respond to emergencies such as floods and earthquakes. The identical satellites orbit Earth 180° apart and at an altitude of almost 700 km, offering a global revisit time of 6-12 days depending on the area (check observation scenario). Sentinel-1’s radar can operate in four modes. The spatial resolution depends on the mode: approx. 5 m x 20 m for IW mode and approx. 20 m x 40 m for EW mode. See [Copernicus services](http://www.esa.int/Our_Activities/Observing_the_Earth/Copernicus/Sentinel-1/) for more details.

#### Vegetation in agriculture algorithms 
 - [Tracking radar vegetation index](sentinel-1/sar_rvi_temporal_analysis)
 - [Agricultural crop monitoring from space](sentinel-1/crop_monitoring)
 - [SAR for deforestation detection](sentinel-1/sar_deforestation_detection)
 - [Radar vegetation index for Sentinel-1 - RVI4S1 script](sentinel-1/radar_vegetation_index)
 - [Radar vegetation index code for dual polarimetric](sentinel-1/radar_vegetation_index_code_dual_polarimetric)

#### Disaster management and prevention algorithms
 - [Seldom and regular water surface detection](sentinel-1/seldom_and_regular_water_surface_detection)
 - [Forest Hurricane](sentinel-1/forest_hurricane)
 - [Flood mapping](sentinel-1/flood_mapping)

#### Urban planning algorithm
 - [Urban areas](sentinel-1/urban_areas)

#### Marine and other water bodies environment algorithms
 - [Water surface roughness visualization](sentinel-1/water_surface_roughness_visualization)
 - [SAR-Ice: A Sea Ice RGB Composite](sentinel-1/sar-ice)

#### Other available scripts
 - [SAR false color visualization](sentinel-1/sar_false_color_visualization)
 - [SAR false color visualization 2](sentinel-1/sar_false_color_visualization-2)

#### Other multi-temporal scripts
  - [SAR multi-temporal backscatter coefficient composite](sentinel-1/sar_multi-temporal_backscatter_coefficient_composite)
  - [Soil Moisture Estimation](sentinel-1/soil_moisture_estimation)
 

## <a name="sentinel-2"></a>Sentinel-2
Dedicated to supplying data for [Copernicus services](http://www.esa.int/Our_Activities/Observing_the_Earth/Copernicus/Sentinel-2), Sentinel-2 carries a multispectral imager with a swath of 290 km. The imager provides a versatile set of 13 spectral bands spanning from the visible and near infrared to the shortwave infrared, featuring four spectral bands at 10 m, six bands at 20 m and three bands at 60 m spatial resolution. As indices primarily deal with combining various band reflectances, the table of 13 bands is given here for reference (see [here](https://sentinel.esa.int/web/sentinel/technical-guides/sentinel-2-msi/msi-instrument){:target="_blank"} for details). The names of the Sentinel-2 bands at your disposal are *B01*, *B02*, *B03*, *B04*, *B05*, *B06*, *B07*, *B08*, *B8A*, *B09*, *B10*, *B11* and  *B12*. 

 - [Sentinel-2 bands](sentinel-2/bands)
 - [Simple RGB composites](sentinel-2/composites)

#### Popular RGB composites
 - [Natural color](sentinel-2/natural_color) product computed correctly to match the color perceived by the human eye.
 - [True color](sentinel-2/true_color) simplistic true color image from red, green and blue bands.
 - [Wildfire visualization](sentinel-2/markuse_fire) (by Pierre Markuse, taken from his [blog post](https://pierre-markuse.net/2017/08/07/visualizing-wildfires-sentinel-2-imagery-eo-browser/){:target="_blank"})

#### Remote sensing indices
 - [False color infrared](sentinel-2/false_color_infrared)
 - [NDVI](sentinel-2/ndvi) - normalized difference vegetation index
 - [NDVI uncertainty](sentinel-2/ndvi_uncertainty) - visualization of uncertainty of NDVI due to uncertainty in band values
 - [collection](sentinel-2/indexdb) of remote sensing indices from an extensive [Index database (IDB)](http://www.indexdatabase.de/){:target="_blank"}
 - [MAX NDVI](sentinel-2/max_ndvi)
 - [ARI](sentinel-2/ari) - anthocyanin reflectance index
 - [mARI](sentinel-2/mari) - modified anthocyanin reflectance index
 - [ARVI](sentinel-2/arvi) - atmospherically resistant vegetation index 
 - [CHL_REDEDGE](sentinel-2/chl_rededge) - chlorophyll red-edge
 - [REDEDGE_POSITION](sentinel-2/red_edge_position) - red edge position index
 - [EVI](sentinel-2/evi) - enhanced vegetation index
 - [EVI2](sentinel-2/evi2) - enhanced vegetation index 2
 - [GNDVI](sentinel-2/gndvi) - green normalized difference vegetation index
 - [MCARI](sentinel-2/mcari) - modified chlorophyll absorption in reflectance index
 - [MSI](sentinel-2/msi) - moisture index
 - [NDMI](sentinel-2/ndmi) - normalized difference moisture index
 - [NDWI](sentinel-2/ndwi) - normalized difference water index
 - [NDMI STRESS](sentinel-2/ndmi_special) - normalized difference moisture index for crop moisture stress
 - [NBR](sentinel-2/nbr) - normalized burn ratio  
 - [NDII](sentinel-2/ndii) - normalized difference 819/1600 NDII
 - [NDCI](sentinel-2/ndci) - normalized difference chlorophyll index
 - [NDSI](sentinel-2/ndsi) - normalised difference snow index  
 - [PSSRB1](sentinel-2/pssrb1) - pigment specific simple ratio for chlorophyll b (800/650 )
 - [SAVI](sentinel-2/savi) - soil adjusted vegetation index
 - [SIPI1](sentinel-2/sipi1) - structure insensitive pigment index
 - [LAI](sentinel-2/lai) - Leaf Area Index
 - [Leaf chlorophyll content](sentinel-2/cab)
 - [Canopy chlorophyll content](sentinel-2/ccc)
 - [FAPAR](sentinel-2/fapar) - the fraction of absorbed photosynthetically active radiation
 - [Color correction with Sentinel Hub](sentinel-2/poor_mans_atcor)
 - [PSRI](sentinel-2/psri) - plant senescence reflectance index
 - [Global mosaic best pixel selection script](sentinel-2/s2gm)
 - [TOA Ratio B09-B8A ColorMap Blue-Red & Natural Colours Script](sentinel-2/ratio_b09-b8a_colormap_blue_red_v0.1)
 - [Tonemapped Natural Color script](sentinel-2/tonemapped_natural_color)
 - [Highlight Optimized Natural Color](sentinel-2/highlight_optimized_natural_color)
 - [Vegetation condition index ](sentinel-2/vegetation_condition_index)
 
#### Cloud detection algorithms
 - [Cohen-Braaten-Yang cloud detection](sentinel-2/cby_cloud_detection/)
 - [Hollstein Clouds, Cirrus, Snow, Shadow, Water and Clear Sky Pixels detection](sentinel-2/hollstein)
 - [Cloudless Mosaic](sentinel-2/cloudless_mosaic)

#### Snow and glaciers algorithms
 - [Snow classifier](sentinel-2/snow_classifier/)
 - [Monthly snow report](sentinel-2/monthly_snow_report)
 - [Snow cover change detection](sentinel-2/snow_cover_change)

#### Disaster management and prevention algorithms
 - [Detecting deep moist convection](sentinel-2/deep_moist_convection)
 - [Fire boundary](sentinel-2/fire_boundary)
 - [burned area index for sentinel-2](sentinel-2/bais2)
 - [Multitemporal burnt area analysis](sentinel-2/burned_area)
 - [Wildfire visualization](sentinel-2/markuse_fire) (by Pierre Markuse, taken from his [blog post](https://pierre-markuse.net/2017/08/07/visualizing-wildfires-sentinel-2-imagery-eo-browser/){:target="_blank"})
 - [Burned Area Visualization](sentinel-2/burned_area_ms)
 
#### Land use/cover classification algorithms
 - [False Color Composite](sentinel-2/false_color_composite)
 - [Barren soil](sentinel-2/barren_soil)
 - [Land Use Visualization for Sentinel-2 Using Linear Discriminant Analysis Script](sentinel-2/land_use_with_linear_discriminant_analysis)

#### Agriculture and forestry algorithms
 - [NDVI anomaly detection](sentinel-2/ndvi_anomaly_detection)
 - [Agricultural growth stage](sentinel-2/agriculture_growth_stage) - multitemporal NDVI 
 - [Forest cut temporal detection](sentinel-2/forest_cut_temporal_detection)
 - [Pseudo forest canopy density (pseudo-FCD)](sentinel-2/pseudo_forest_canopy_density)
 - [Infrared agriculture display](sentinel-2/infrared_agriculture_display)

#### Marine and other water bodies environment algorithms
 - [White-water detection](sentinel-2/white_water)
 - [Ocean plastic detector prototype](sentinel-2/ocean_plastic_detector)
 - [Ulyssys Water Quality Viewer](sentinel-2/ulyssys_water_quality_viewer) - chlorophyll and suspended sediment for water quality visualization
 - [Satellite Derived Bathymetry Mapping - SDBM](sentinel-2/satellite_derived_bathymetry_mapping-sdbm)
 - [Aquatic Plants and Algae Custom Script Detector (APA Script)](sentinel-2/apa_script)
 - [se2waq](sentinel-2/se2waq) - water quality for Sentinel-2
 - [Water In Wetlands Index (WIW)](sentinel-2/wiw_s2_script)

#### Urban planning algorithms
 - [Green city](sentinel-2/green_city)
 - [City highlights](sentinel-2/city_highlights)
 - [Urban land infrared color](sentinel-2/urban_land_infrared)
 - [Urban classified](sentinel-2/urban_classified)
 
#### Other multi-temporal scripts
 - [Monthly composite](sentinel-2/monthly_composite)
 - [Water Bodies Mapping - WBM](sentinel-2/water_bodies_mapping-wbm)

#### Other available scripts
 - [Selective Enhancement based on Indices](sentinel-2/selective_enhancement_based_on_indices)
 - [Homage to Mondrian](sentinel-2/homage_to_mondrian) - artistic script
 - [Index visualisation](sentinel-2/index_visualization) - universal script for visualisation of indices
 - [NDVI on L2A Vegetation and natural Colours](sentinel-2/ndvi-on-vegetation-natural_colours)

## <a name="sentinel-3"></a>Sentinel-3 OLCI

Sentinel-3 is a low Earth-orbit moderate size satellite compatible with small launchers including VEGA and ROCKOT. The main objective of the mission is to measure sea surface topography, sea and land surface temperature, and ocean and land surface color with high accuracy and reliability to support ocean forecasting systems, environmental monitoring and climate monitoring. Ocean and Land Colour Instrument (OLCI) provides a set of 21 bands ranging from the visible to the near infrared light (400 nm < λ< 1 020 nm). The Sentinel-3 provides imagery in 300 m spatial resolution. Sentinel-3 OLCI instrument ensures continuity of the ENVISAT MERIS.

 - [Sentinel-3 OLCI bands](sentinel-3/bands)
 - [Simple RGB composites](sentinel-3/composites)

#### Enhanced true color scripts
 - [Enhanced true color](sentinel-3/enhanced_true_color)
 - [Enhanced true color-2](sentinel-3/enhanced_true_color-2)
 - [Tristimulus](sentinel-3/tristimulus)
 
#### Remote sensing indices
 - [OTCI](sentinel-3/otci) - Terrestrial chlorophyll index
 - [Ulyssys Water Quality Viewer](sentinel-2/ulyssys_water_quality_viewer) - chlorophyll and suspended sediment for water quality visualization
 - [NDBI](sentinel-3/ndbi) - Normalized Bare ice Index

#### Other available scripts
 - [OLCI Natural Colours with Sigmoid](sentinel-3/natural_colors_sigmoid)

## <a name="sentinel-5P"></a>Sentinel-5P

Sentinel-5P provides atmospheric measurements, relating to air quality, climate forcing, ozone and UV radiation with high spatio-temporal resolution. Its data is used for monitoring of concentrations of carbon monoxide (CO), nitrogen dioxide (NO2) and ozone (O3) in air as well as for monitoring of UV aerosol index (AER_AI) and different geophysical parameters of clouds (CLOUD). EO Browser serves level 2 geophysical products. The TROPOspheric Monitoring Instrument (TROPOMI) on board of the satellite operates in the ultraviolet to shortwave infrared range with 7 different spectral bands: UV-1 (270-300nm), UV-2 (300-370nm), VIS (370-500nm), NIR-1 (685-710nm), NIR-2 (755-773nm), SWIR-1 (1590-1675nm) and SWIR-3 (2305-2385nm). Its spatial resolution is below 8km for wavelengths above 300nm and below 50km for wavelength below 300nm. It covers almost the whole globe (95 % coverage for latitudes in the interval [-7°, 7°]).

#### Available scripts
 - [Nitrogen Dioxide tropospheric column](sentinel-5p/nitrogen_dioxide_tropospheric_column)

## <a name="landsat-8"></a>Landsat 8
The Landsat program is the longest running enterprise for acquisition of satellite imagery of Earth, running from 1972. The most recent, [Landsat 8](http://landsat.usgs.gov/landsat8.php){:target="_blank"}, was launched on February 11, 2013. Landsat-8 data has 11 spectral bands with spatial resolutions ranging from 15 to 60 meters. The names of the Landsat-8 bands at your disposal are *B01*, *B02*, *B03*, *B04*, *B05*, *B06*, *B07*, *B08*, *B09*, *B10* and *B11*.

 - [Landsat 8 bands](landsat-8/bands)
 - [Simple RGB composites](landsat-8/composites)

#### Remote sensing indices
  - [collection](landsat-8/indexdb) of remote sensing indices from an extensive [Index database (IDB)](http://www.indexdatabase.de/){:target="_blank"}
  - [Build-up index](landsat-8/built_up_index)
  - [NDVI](landsat-8/ndvi)

#### Other available scripts
  - [Land surface temperature (LST) mapping](landsat-8/land_surface_temperature_mapping)
  - [Water In Wetlands Index](landsat-8/wiw_L8_script)

## <a name="landsat-57"></a>Landsat 5 and 7

Landsat 7 and the retired Landsat 5 orbit's are sun-synchronous, with near-polar orbits, flying at an altitude of 705 km (438 mi). Landsat 5 long outlived its original three-year design life. Developed by NASA and launched in 1984, Landsat 5 has orbited the planet over 150,000 times while transmitting over 2.5 million images land surface images around the world. The Landsat 7 satellite still orbits the the Earth in a sun-synchronous, near-polar orbit, at an altitude of 705 km (438 mi). The satellites are multispectra, providing visible, near infrared, mid infrared and thermal bands. 

For more on Landsat 5, including its available bands, read [here](https://www.usgs.gov/land-resources/nli/landsat/landsat-5?qt-science_support_page_related_con=0#qt-science_support_page_related_con){:target="_blank"} and for Landsat 7, read [here.](https://www.usgs.gov/land-resources/nli/landsat/landsat-7?qt-science_support_page_related_con=0#qt-science_support_page_related_con){:target="_blank"}. 

- [Landsat 5 and 7 bands](Landsat-57/bands)
- [Simple RGB composites](Landsat-57/composites)
 
## <a name="modis"></a>MODIS
The Moderate Resolution Imaging Spectroradiometer (MODIS) MCD43A4 version 6 on Sentinel Hub is hosted at Amazon Web Services (AWS). Dataset is updated daily and provides the 500 meter Nadir Bidirectional reflectance distribution function Adjusted Reflectance (NBAR) data of MODIS "land" bands 1-7: *B01*, *B02*, *B03*, *B04*, *B05*, *B06* and *B07*.

  - [MODIS bands](modis/bands)

#### Remote sensing indices
  - [collection](modis/indexdb) of remote sensing indices from an extensive [Index database (IDB)](http://www.indexdatabase.de/){:target="_blank"}
  
## <a name="planet_scope"></a>PlanetScope (Commercial)

<a href="https://www.planet.com/products/monitoring/">PlanetScope</a> satellite constellation consists of more than 130 small satellites called Doves. The satellites are launched in groups, which constantly improves mission's characteristics such as revisit times, spatial and spectral resolutions. PlanetScope data complements Sentinel-2 with better spatial resolution (3m) and almost global daily coverage. It is an excellent source for vegetation monitoring. For more information on PlanetScope, visit our <a href="https://docs.sentinel-hub.com/api/latest/#/data/PlanetScope">documentation page</a>. 

The spectral bands of PlanetScope data are the following: 

*B1 - Blue, resolution 3m*

*B2 - Green, resolution 3m*

*B3 - Red, resolution 3m*

*B4 - Near Infrared, resolution 3m*

 - [True Color](planet_scope/true_color)
 - [False Color](planet_scope/false_color)
 - [NDVI](planet_scope/ndvi)
 - [NDWI](planet_scope/ndwi)
 - [Green City](planet_scope/green_city)
 
## <a name="airbus_pleiades"></a>Airbus Pleiades (Commercial)

<a href="https://www.intelligence-airbusds.com/en/8692-pleiades">Pléiades</a> constelation is composed of two twin satellites orbiting the Earth 180° apart. The satellites deliver the incredible global 0.5 m spectral resolution imagery. Pleiades' satellites share the orbit with SPOT satellites, which makes it possible to combine the data form both sources.
The Pléiades data with its high spatial resolution is suitable for a wide range of remote sensing applications such as vegetation monitoring, precise mapping, as well as risk and disaster management. To learn more about Pleiades, visit our <a href="https://docs.sentinel-hub.com/api/latest/#/data/Airbus-Pleiades"> documentation page.</a> 

The spectral bands of Pleiades data are the following: 

*B0 - Blue (430-550 nm,	resolution 2m)*

*B1 - Green (490-610 nm, resolution	2m)*

*B2 - Red (600-720 nm), resolution 2m*	

*B3 - Near Infrared (750-950 nm), resolution 2m*

*PAN	- Panchromatic (480-830 nm), resolution 0.5m*

Pleiades's RGB bands are in 2 meter spatial resolution. To take advantage of the 0.5 m PAN band, the pansharpening process is required. 
 
 - [True Color](airbus_pleiades/true_color)
 - [Pansharpened True Color](airbus_pleiades/true_color_pansharpened)
 - [False Color](airbus_pleiades/false_color)
 - [NDVI](airbus_pleiades/ndvi)
 - [NDWI](airbus_pleiades/ndwi)
 - [Green City](airbus_pleiades/green_city)
 - [Pansharpened Green City](airbus_pleiades/green_city_pansharpened)

# <a name="howto"></a>Adding new custom scripts
Have a look at the [template](example) and follow the procedure described there.  

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">
<img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>
<br />
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
