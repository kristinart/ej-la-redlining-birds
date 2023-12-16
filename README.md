# Environmental justice impacts of historical redlining in Los Angeles County

This repository contains an analysis of community characteristics at the census block group level in Los Angeles County. In this analysis, we summarize and visualize present-day environmental and health hazards across space and determine whether the patterns share a relationship with two additional variables: historic Home Owners' Loan Corporation (HOLC) grades and 2022 bird observations. This analysis indicates that HOLC grades and the historic practice of redlining have influenced the socioeconomic and environmental characteristics of present-day neighborhoods, which aligns with the literature.

The structure and contents of the repository are shown below:

> ```         
> ej-la-redlining-birds
> ├── README.md
> ├── data
> │   ├── EJSCREEN_2023_BG_Columns.xlsx      #metadata for EJScreen parameters
> │   ├── EJSCREEN_2023_BG_StatePct_with_AS_CNMI_GU_VI.gdb      #EJScreen geodatabase
> │   ├── ejscreen-tech-doc-version-2-2.pdf     #technical support document for EJScreen,
> │   └── gbif-birds-LA     #geospatial data on bird observations during 2022
> │       ├── gbif-birds-LA.dbf
> │       ├── gbif-birds-LA.prj
> │       ├── gbif-birds-LA.shp
> │       └── gbif-birds-LA.shx
> ├── ej-la-redlining-birds.Rproj
> ├── figures
> │   ├── la_holc_bird_observations.png     #bar chart of bird observations by HOLC grade
> │   ├── la_holc_grades_map.png            #map of HOLC neighborhoods in LA county
> │   └── la_wastewater_discharge_map.png   #map of wastewater discharge in LA county    
> └── scripts
>     ├── la_redlining_biodiversity.Rmd     #analysis Rmarkdown document
>     └── la_redlining_biodiversity.html    #analysis html document
> ```

### Data

The data used in this analysis are too large to include in the repository and instead can be downloaded from [here](https://drive.google.com/file/d/1lcazRbNSmP8Vj9sH1AIJcO4D1d_ulJij/view?usp=share_link). The data sources are described below:

#### *EJScreen*

We utilized data from the United States Environmental Protection Agency's (US EPA) EJScreen: Environmental Justice Screening and Mapping Tool. The tool was created for community residents and other stakeholders to easily access environmental and demographic information [(US EPA)](https://www.epa.gov/ejscreen/purposes-and-uses-ejscreen). It is also used to support a wide range of research and policy questions, particularly with regards to environmental justice. We utilize environmental and demographic information reported at the [block group](https://en.wikipedia.org/wiki/Census_block_group) level downloaded from the [EPA site](https://www.epa.gov/ejscreen/download-ejscreen-data).

#### *Mapping Inequality*

We utilize digitized maps and information from the HOLC that were developed by a team of researchers at the University of Richmond. This effort was led by the [Digital Scholarship Lab](https://dsl.richmond.edu/) and is part of the [Mapping Inequality](https://dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58) project. In particular, we used a map of HOLC grade designations in Los Angeles County. Information about the data can be found [here](https://dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58&text=downloads).

#### *Biodiversity Observations*

We utilized observations of biodiversity in Los Angeles County that were sourced from the [Global Biodiversity Information Facility](gbif.org), which is the largest aggregator of biodiversity observations in the world. The observation data include the date and species the observed organisms. For our analysis, we utilize bird observations in 2022.

### References

Ellis-Soto, D., Chapman, M., & Locke, D. H. (2023). Historical redlining is associated with increasing geographical disparities in bird biodiversity sampling in the United States. Nature Human Behaviour, 1-9. [DOI: 10.1038/s41562-022-01389-3]

Gee, G. C. (2008). A multilevel analysis of the relationship between institutional and individual racial discrimination and health status. American Journal of Public Health, 98(Supplement_1), S48-S56. [DOI: 10.2105/AJPH.98.Supplement_1.S48]

Hoffman, J. S., Shandas, V., & Pendleton, N. (2020). The effects of historical housing policies on resident exposure to intra-urban heat: A study of 108 US urban areas. Climate, 8(1), 12. [DOI: 10.3390/cli8010012]

Nardone, A., Rudolph, K. E., Morello-Frosch, R., & Casey, J. A. (2021). Redlines and greenspace: The relationship between historical redlining and 2010 greenspace across the United States. Environmental Health Perspectives, 129(1), 017006. [DOI: 10.1289/EHP6729]

Nelson, R. K., Winling, L., Marciano, R., Connolly, N., et al. (n.d.). Mapping Inequality. American Panorama, Eds. R. K. Nelson & E. L. Ayers. Retrieved October 17, 2023, from <https://dsl.richmond.edu/panorama/redlining/>
