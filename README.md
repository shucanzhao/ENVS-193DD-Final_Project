# ENVS 193DD Final Project

**Spring 2026**

## General information

This repository contains the final project for the Water Warriors group in ENVS 193DD. The project analyzes dissolved oxygen patterns in NCOS water quality monitoring data.

Group members:

- Phoebe Dupa
- Rebecca Martinez
- Shucan Zhao

The main questions are:

- How does dissolved oxygen differ across sites?
- How does dissolved oxygen differ across elevation-code measurement positions?
- Is dissolved oxygen related to water temperature?

To run the code in this repository, the following packages are needed:

```r
library(tidyverse)
library(janitor)
library(here)
library(lubridate)
```

## Repository structure

```text
.
├── README.md
├── ENVS-193DD-Final_Project.Rproj
├── code
│   ├── final_paper.qmd
│   ├── final_paper.pdf
│   ├── final_visual_draft.qmd
│   ├── final_visual_draft.pdf
│   ├── ecology.csl
│   ├── references.bib
│   ├── visual_draft_2.qmd
│   ├── visual_draft_2.pdf
│   ├── visual_draft-3.qmd
│   ├── visual_draft-3.pdf
│   ├── Visualization_Draft.qmd
│   └── Visualization_Draft.pdf
├── data
│   ├── NCOS_YSI_Water_Quality_Monitoring_0.csv
│   ├── YSI_Data_Begin_1.csv
│   └── NOAA-weather-data.csv
└── images
    ├── do_across_sites.png
    ├── do_stratification_by_site.png
    ├── do_elevation_profile_by_site.png
    ├── median_do_through_time_by_elevation.png
    ├── do_time_exploration.png
    ├── temp_time_exploration.png
    └── mockup_plot.png
```


### Code and output files

- `Visualization_Draft.qmd`: Shucan’s visualization draft
- `Visualization_Draft.pdf`: rendered PDF version of Shucan’s visualization draft

- `visual_draft_2.qmd`: Rebecca’s visualization draft
- `visual_draft_2.pdf`: rendered PDF version of Rebecca’s updated visualization draft

- `visual_draft-3.qmd`:Phoebe's visualization draft
- `visual_draft-3.pdf`: rendered PDF version of Phoebe’s updated visualization draft


### Data files

The project uses three datasets:

- `NCOS_YSI_Water_Quality_Monitoring_0.csv`: metadata for each water quality survey, including site name, monitoring date, weather notes, and location information
- `YSI_Data_Begin_1.csv`: water quality measurements collected during each survey, including dissolved oxygen, temperature, salinity, conductivity, and elevation code
- `NOAA-weather-data.csv`: daily weather data, including precipitation, maximum temperature, and minimum temperature

## Project workflow

The project includes:

- cleaning the weather, metadata, and water parameter datasets
- joining metadata and water quality measurements by survey ID
- joining weather data by date
- filtering to the three main NCOS sites, 2024 and 2025 water years, and elevation codes 0–2
- summarizing dissolved oxygen by site and elevation code
- visualizing dissolved oxygen across sites, elevation codes, and temperature
- testing group differences with Kruskal-Wallis and pairwise Wilcoxon tests
- testing temperature relationships with linear models

## Rendered output

- [Final paper](https://github.com/shucanzhao/ENVS-193DD-Final_Project/blob/main/code/final_paper.pdf)
- [Final visual draft](https://github.com/shucanzhao/ENVS-193DD-Final_Project/blob/main/code/final_visual_draft.pdf)
- [Visual draft 3](https://github.com/shucanzhao/ENVS-193DD-Final_Project/blob/main/code/visual_draft-3.pdf)
- [Visual draft 2](https://github.com/shucanzhao/ENVS-193DD-Final_Project/blob/main/code/visual_draft_2.pdf)
- [Visualization draft](https://github.com/shucanzhao/ENVS-193DD-Final_Project/blob/main/code/Visualization_Draft.pdf)


## Project roles

- Natural history/framing director: Phoebe Dupa
- Stats and visualization director: Rebecca Martinez
- GitHub/code director: Shucan Zhao

## Elective

The group plans to create a visual model using three clear containers to represent the three sampling sites. Blue beads will represent water, and white beads will represent dissolved oxygen patterns or stratification at each site.

The cylinder containers and beads have already been purchased. Once the final visuals are planned, the group can use the beads to recreate the dissolved oxygen patterns observed at each site.

## Repository links

- [Final project repository](https://github.com/shucanzhao/ENVS-193DD-Final_Project)
- [Project proposal repository](https://github.com/shucanzhao/project-proposal)
- [Literature Dissection](https://github.com/shucanzhao/literature-dissection)
