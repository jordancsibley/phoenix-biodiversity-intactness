# Biodiversity Intactness Index change in Phoenix, AZ
![Phoenix suburb in development](https://www.coxblue.com/wp-content/uploads/multihousing_arizona-2048x1152.jpg)
Phoenix, AZ suburb neighborhood.  Source: CoxBLUE
## About 

This notebook aims to investigate the impacts of urban expansion on biodiversity in the Phoenix metropolitan area by analyzing changes in the Biodiversity Intactness Index (BII) between 2017 and 2020. Through the analysis of BII data for Phoenix, this notebook will explore the extent of urbanization's effect on biodiversity, focusing on the percentage of land with high BII scores (indicating intact ecosystems). By comparing the BII values in 2017 and 2020, we will gain insights into how the ecological landscape has changed. 

## Analysis Highlights 
- **Data Access**: Accessed Biodiversity Intactness Index (BII) data from the Microsoft Planetary Computer using the STAC `Client` and `planetary_computer` package.
- **Geospatial Data Wrangling**: Performed data wrangling on raster data with `rioxarray` for clipping and CRS alignment, and computed BII changes between 2017 and 2020.
- **Visualization**: Created customized maps using `matplotlib`, including setting colorbars and legends to display BII data and highlight areas of biodiversity loss.

## Data Access
- **[Biodiveristy Intactness Index (BII) Time Series](https://planetarycomputer.microsoft.com/dataset/io-biodiversity)**: This data comes from the Microsoft Planetary Computer STAC catalog. The `io-biodiveristy` collection of this catalog includes global terrestrial biodiversity intactness at 100m resolution for years 2017-2020.
- **[Phoenix Subdivision Shapefile](https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2020&layergroup=County+Subdivisions)**: This data comes from the United States Census 2020 TIGER/Line® Shapefiles. 

## Repository Structure 
The notebook `BII-phoenix.ipynb` contains all the analysis for this project. The `data` folder contains the shapefiles for the Arizona county subdivisions. 
```
phoenix-biodiversity-intactness
│   README.md
|   .gitignore
│   BII-phoenix.ipynb
└───data
    │ tl_2020_04_cousub.cpg
    │ tl_2020_04_cousub.dbf
    │ tl_2020_04_cousub.prj
    │ tl_2020_04_cousub.shp
    │ tl_2020_04_cousub.shp.ea.iso.xml
    │ tl_2020_04_cousub.shp.iso.xml
    │ tl_2020_04_cousub.shx
```
## Author 

Jordan Sibley 

Master of Environmental Science Student at the Bren School of Environmental Science & Management

jcsibley@bren.ucsb.edu

jordan.c.sibley@gmail.com 

## Acknowledgments

The material for this assignment was presented by Dr. Carmen Galaz García in the course Working with Environmental Datasets (EDS 220) at the Bren School of Environmental Science & Management, Fall 2024. The assignment description can be found [here](https://meds-eds-220.github.io/MEDS-eds-220-course/assignments/final-project.html).

## References 
Impact Observatory (2022), Biodiversity Intactness [Data file]. Planetary Computer STAC API. https://planetarycomputer.microsoft.com/dataset/io-biodiversity

US Census Bureau (2020), 2020 Tiger/Line Shapefiles:County Subdivisions [Data file]. https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2020&layergroup=County+Subdivisions 
