# Seattle_Crime_Analysis


## Table of Contents
- [Table of Contents](#table-of-contents)
- [Requirements](#requirements)
- [Dataset](#dataset)
- [References](#references)
- [Authors](#authors)

## Requirements
[(Back to top)](#table-of-contents)  
This project utilize Python libraries like Pandas, Numpy for data manipulation, Altair for visualization., Geopanda and Folium for geospatial visualization
Make sure you have the following Python libraries installed:

```bash
pip install pandas altair 
```

## Dataset:
[(Back to top)](#table-of-contents)  
The analysis relies on crime data acquired from the Seattle Police Department, covering the period from 2008 to 2022. Each crime report is uniquely identified by a Report Number, and are categorized by both specific Offense Types and broader Offense Parent Groups. Notably, due to the granularity of Offense Types, the report opts for Offense Parent Groups to streamline the crime classification.

Each incident is associated with start time, end time, and report time, with a preference for using the reported time for filtering as incidents are considered finalized at that point. Additionally, incidents are geographically tagged with coordinates and various location identifiers such as police precincts, beats, and sectors. To ensure public understanding, the analysis utilizes Community Reporting Areas (CRAs) in Seattle, which delineate neighborhoods and neighborhood districts,providing a more accessible language. These CRAs aggregate smaller zoning areas like Census tracts and blocks, ensuring precise reporting without overlaps. Data from the Census Bureau are pulled in for these smaller area characteristics and geometry.

The incident coordinates undergo transformation into Geometry point objects, facilitating a spatial join technique to determine the larger zoning areas to which each point belongs. Subsequently, a merger is conducted with the "Selected Demographic and Housing Estimates (DP05)" data for the year 2020, incorporating geo spatial population information. The combination of crime patterns with demographic factors provides valuable insights, enriching the understanding of the socio-economic landscape in Seattle.

Seattle Police Department Crime Data: https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5  
Seattle Demogrphic Data: https://data-seattlecitygis.opendata.arcgis.com/datasets/SeattleCityGIS::selected-demographic-and-housing-estimates-dp05/explore  
Seattle Community Areas Geospatial data: https://data-seattlecitygis.opendata.arcgis.com/datasets/SeattleCityGIS::community-reporting-areas-3/about  
Seattle Census Block data: https://data.seattle.gov/dataset/2020-Census-Blocks-Seattle/rg9f-z788/data  


## References:
[(Back to top)](#table-of-contents)  


## Authors
[(Back to top)](#table-of-contents)

- [@Akanksha Sharma](https://github.com/akankshasharmadid)
    [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/akanksha-12831bb1)
    [![Leetcode](https://img.shields.io/badge/LeetCode-000000?style=for-the-badge&logo=LeetCode&logoColor=#d16c06)](https://www.leetcode.com/akanksha185/)

- [@Kewal Tadas ](https://github.com/kewal97)
    [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kewaltadas/)
- [@Taylor ](https://github.com/tuananhnguyen527)
    [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/taylor527/)
