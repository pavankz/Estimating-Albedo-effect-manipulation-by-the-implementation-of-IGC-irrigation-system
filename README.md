# Estimating-Albedo-effect-manipulation-by-the-implementation-of-IGC-irrigation-system using google earth engine
This work looks into effects of the river system in an arid region using google earth engine and landsat data series.
Find the related work in [Google Earth Engine]()

**Objective:**
1. Impact of Indira Gandhi Canal network on regional climate, Bikaner Tahsil, Rajasthan
2. Estimating of Albedo from [Landsat TM](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LT05_C02_T1_L2) and [Landsat OLI](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C02_T1_L2) and establishing realtion with Land surface temperature (LST) and Normalized Difference Vegetation Index (NDVI) from 1990 to 2024
3. Temporal land use and land cover (LULC) analysis of Bikaner Tahsil during 1990 to 2023
4. Impact of land use on albedo and precipitation pattern 

**Analysis**
- The Estimation of [albedo](https://ieeexplore.ieee.org/abstract/document/7976307), [LST](https://www.sciencedirect.com/science/article/pii/S2352938521002019) and [NDVI](https://www.researchgate.net/profile/Jan-Niklas-Schmid/publication/320708352_Using_Google_Earth_Engine_for_Landsat_NDVI_time_series_analysis_to_indicate_the_present_status_of_forest_stands/links/5d29201b458515c11c2ab18e/Using-Google-Earth-Engine-for-Landsat-NDVI-time-series-analysis-to-indicate-the-present-status-of-forest-stands.pdf) carried out using [GEE](https://earthengine.google.com/) and [QGIS](https://qgis.org/download/)
- The Land use classification also done in GEE using [Random Forest Classification](https://www.mdpi.com/2072-4292/14/11/2654) 
- To identify relation between albedo, ndvi and LST, creaed 1000 sample points on the raster files and extracted associated values in GEE to carry out correlation analysis by Ordinary Least Squares using Statsmodels.api in jupyter notebook
- The Precipitation maps and time series ploted from [CHIRPS](https://developers.google.com/earth-engine/datasets/catalog/UCSB-CHG_CHIRPS_PENTAD) and [TRMM](https://developers.google.com/earth-engine/datasets/catalog/TRMM_3B43V7) datasets
