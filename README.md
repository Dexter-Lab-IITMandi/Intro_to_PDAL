[![NSF-1642611](https://img.shields.io/badge/NSF-1642611-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1642611) [![NSF-1948994](https://img.shields.io/badge/NSF-1948994-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1948994) [![NSF-1830734](https://img.shields.io/badge/NSF-1830734-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1830734)

# Introduction to PDAL
This tutorial was provided as part of a training session at the [EarthCube Advancing the Analysis of HRT Workshop #2](https://opentopography.org/workshops/earthcube-advancing-analysis-hrt-workshop-2) from May 8-10, 2023 at Arizona State University. The intended audience is users who have either never used [PDAL](https://pdal.io/en/latest/) or are novice users.  This tutorial will focus on basic syntax and some simple workflows to get
users familiar with working from PDAL.  Topics include:
- Working with pipelines
- Learning how to interrogate point clouds with PDAL (e.g. metadata, basic stats, etc.)
- Pre-processing datasets (e.g. thinning, filtering, etc.)
- Creating ground-classified datasets
- Gridding point clouds into Digital Elevation Models (DEMs)
- Generating DEM derviatives and computing differences between DEMs with GDAL

# Tutorial Preparation
- Users should follow the instructions on the document [Installation.md
](./Installation.md) to install the necessary and recommended software.

# Tutorial Structure
- The tutorial is based on the series of markdown documents in the repo.  Users are expected to have a working copy of PDAL running on their system so that they can copy/paste and experiment with commands on their local PDAL installation.
- Sample PDAL pipelines that are discussed in the docs are available in the pipelines folder.  
- There is a basic bash-based Jupyter Notebook available for users who are more comfortable working in the Jupyter environment. It contains many of the commands that are presented in the docs, and is intended as another pathway for users to get more comfortable with working with PDAL. 

## Tutorial Contents
- PDAL Overview
- [Introduction to PDAL - Part 1](./IntrotoPDAL_Part1.md)
  - PDAL mechanics & basic commands
  - Inspecting point cloud files with PDAL

- [Introduction to PDAL - Part 2](./IntrotoPDAL_Part2.md)
  - File I/O
  - Reprojections
  - Filter operations
  - Creating dataset boundaries

- [Introduction to PDAL - Part 3](./IntrotoPDAL_Part3.md)
  - Point Cloud Visualization
  - Data preparation (e.g. noise filtering)
  - Creating Ground Classifications (e.g. SMRF filters)

- [Introduction to PDAL - Part 4](./IntrotoPDAL_Part4.md)
  - Gridding point clouds
  - GDAL: Raster Math & visualization

- Optional: [Accessing USGG 3DEP EPT data via AWS](AccessUSGS3DEPEntwine.md)


# Example datasets
- There are some example [LAZ](https://laszip.org/) files under the data directory of the git repo.  However, users are also encouraged to use their own data, or download data from [OpenTopography](https://portal.opentopography.org/datasets).  **Note** for the workshop, it is best to work with smaller files to keep processing times short.  As a rule of thumb, keeping datasets below 5 million points is recommended for quick processing times.

# Acknowledgements 
The primary aim of this tutorial is to get users comfortable with basic PDAL commands, and workflows. This tutorial is geared to the novice PDAL user. Content for this workshop is based on a subset of two prior existing PDAL workshops:
- PDAL's main workshop material: https://pdal.io/en/2.5.3/workshop/index.html
- Dr. Adam Steer's PDAL workshop from FOSS4G SotM Oceania in 2018: https://github.com/adamsteer/f4g-oceania-pdal

Users are encouraged to explore these two excellent resources for more advanced PDAL usage and examples.
