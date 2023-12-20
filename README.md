# Seattle_Crime_Analysis


## Table of Contents
- [Table of Contents](#table-of-contents)
- [Requirements](#requirements)
- [Dataset](#dataset)
- [References](#references)
- [Authors](#authors)


## Requirements
[(Back to top)](#table-of-contents)  
Make sure you have the following Python libraries installed:

```bash
pip install pandas altair
```

## Dataset
[(Back to top)](#table-of-contents)  
About Dataset
The analysis utilizes crime data sourced from the Seattle Police Department spanning the years 2008 to 2022, available at https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5. The dataset encompasses a comprehensive array of information crucial for understanding and analyzing criminal activities. Each crime report is uniquely identified by a Report Number, facilitating tracking and reference, while the Offense ID serves as an added unique identifier for individual offenses. The temporal aspects of the offenses are detailed through Offense Start date and end date, providing insights into the duration of events. 

The dataset obtained from SPD contained longitude and latitude coordinates which doesn’t provide any higher level meaning in terms of geographic crime pattern. These coordinates were transformed into Geometry point objects, then employing a spatial join technique, each point was linked to its respective Census Block using Seattle's 2020 Census Block geometry data.  Leveraging the hierarchical structure of Census Blocks and Tracts within larger areas, the data was further contextualized within Community Reporting Areas (CRAs) in Seattle. CRAs, resembling neighborhood and neighborhood districts, provide a localized community-level perspective, aligning with familiar terminology for Seattle residents. Additionally, Seattle's neighborhoods and neighborhood districts are aligned with census tracts borders, ensuring a non-overlapping dataset for accuracy. Subsequently, a merger with "Selected Demographic and Housing Estimates (DP05)" data for the 2020 population was executed, contributing to a more nuanced analysis of normalization by population or by areas. This integrated approach offers valuable insights into the interplay between crime patterns and demographic factors, enhancing the overall understanding of the socio-economic landscape.

The rationale behind aggregating points into larger areas is twofold: it provides a summarized view of crime patterns in multi-level while retaining the localization of incidents. Additionally, employing familiar terms caters to the understanding and engagement of our Seattle audience. 

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
