# Visualizing the Thomas Fire Scar and AQI in Santa Barbara and Ventura County
![thomas fire image](https://ca-times.brightspotcdn.com/dims4/default/13305b6/2147483647/strip/true/crop/2048x1365+0+0/resize/1440x960!/quality/75/?url=https%3A%2F%2Fcalifornia-times-brightspot.s3.amazonaws.com%2F76%2F08%2F7f21ae4862f56a40e34faa951a9f%2Fla-me-thomas-fire-photos-013)
Image credits: [Los Angeles Times](https://www.latimes.com/local/lanow/la-me-thomas-fire-photos-photogallery.html)

This repository explores the effects of the 2017 Thomas Fire in California by using open access AQI data, Landsat data and fire perimeter geospatial data. The Thomas Fire, which burned over 280,000 acres in Ventura and Santa Barbara counties in December 2017, was one of California’s largest wildfires at the time. It caused widespread ecological damage, displaced communities, and left lasting environmental impacts. This repository houses a Jupyter Notebook (`thomas-aqi.ipynb`) examining the change in air quality before and after the fire. The next notebook (`false-color-image.ipynb`) visualizes a false color image of the Thomas Fire in combination with the fire's boundary. The last notebook (`complete-thomas-fire-analysis.ipynb`) synthesizes both of these analyses together into one streamlined workflow. 

## Description
File map
```
├── data
│   ├── thomas_boundary.geojson               # fire perimeter data
│   └── landsat8-2018-01-26-sb-simplified.nc  # landsat data
├── .gitignore
├── README.md
├── complete-thomas-fire-analysis.ipynb      # complete analysis for blog post
├── false-color-imagery.ipynb                # false color analysis
└── thomas-aqi.ipynb                         # aqi analysis
```

## Data access
Data in this project were pulled from  
- Air Quality Index (AQI): [US Environmental Protection Agency](https://www.airnow.gov/aqi/aqi-basics/) 
- Landsat: [Microsof Planetary Computer data catalogue](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2)
- Fire Perimeter: [CalFire](https://www.fire.ca.gov/what-we-do/fire-resource-assessment-program/fire-perimeters)

The data necessary for this project can be found under the `data` folder located in the repository. 

## References

AQI data:
- US Environmental Protection Agency. Air Quality System Data Mart AirNow available via https://www.epa.gov/outdoor-air-quality-data. Accessed October 17 2024.

Landsat data:
- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 4-5 Thematic Mapper Level-2, Collection 2 [dataset]. U.S. Geological Survey. https://doi.org/10.5066/P9IAXOVV
- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 7 Enhanced Thematic Mapper Plus Level-2, Collection 2 [dataset]. U.S. Geological Survey. https://doi.org/10.5066/P9C7I13B
- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [dataset]. U.S. Geological Survey. https://doi.org/10.5066/P9OGBGM6 

Fire Perimeter data:
- California Department of Forestry and Fire Protection (CAL FIRE), [calfire_all.gdb], [2024-11-17], retrieved from [CAL FIRE data portal](https://www.fire.ca.gov/what-we-do/fire-resource-assessment-program/fire-perimeters).


## Acknowledgements
All materials were created by [Carmen Galaz-Garcia](https://github.com/carmengg) for [EDS-220: Working with Environmental Data](https://meds-eds-220.github.io/MEDS-eds-220-course/).

