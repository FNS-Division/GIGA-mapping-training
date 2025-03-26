# GIGA-mapping-training

![Logo](https://www.itu.int/web/pp-18/assets/logo/itu_logo.png)

![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg) 
[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/)
[![QGIS](https://img.shields.io/badge/QGIS-589632.svg?style=flat&logo=QGIS&logoColor=white)](https://qgis.org/)

Training materials for an ITU course provided as part of the following event focusing on network infrastructure analysis and planning:

[Infrastructure mapping for school connectivity](https://academy.itu.int/training-courses/full-catalogue/infrastructure-mapping-school-connectivity), Geneva – Switzerland, 27-28 February 2025

<a href="https://ibb.co/yW090yp"><img src="https://i.ibb.co/4PWqWT2/windhoek-fiber.png" alt="windhoek-fiber" border="0"></a>

_Figure: Fiber path simulation in Windhoek, Namibia_

## Table of Contents

1. [Overview](#overview)
2. [Data](#data)
  - [Data Repository](#data-repository)
  - [Data Sources](#data-sources)
3. [Training Agenda](#training-agenda)
4. [Prerequisites](#prerequisites)
  - [For Google Colab Users](#for-google-colab-users)
  - [For Local Setup](#for-local-setup)
5. [Setup Instructions](#setup-instructions)
  - [To Run Notebooks Locally](#to-run-notebooks-locally)
  - [To Run Notebooks on Google Colab](#to-run-notebooks-on-google-colab)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

## Overview

This repository contains links to course slides hosted on a [Google Drive folder](https://drive.google.com/drive/folders/1AEt-lrxRcV2G_SAfA0isPpj6omJ7M7Qr?usp=drive_link), Jupyter notebooks and supporting materials for 2-day course on infrastructure mapping and analysis.

The course will introduce the methodology used by the International Telecommunication Union (ITU) to measure gaps in ICT infrastructure and for connectivity business planning.  It aims to improve the theoretical and practical skills of participants in collecting ICT infrastructure data, identifying underserved areas, applying GIS tools, and using connectivity models to test and compare selected connectivity scenarios. 

During practical hands-on sessions, participants will learn how to source and prepare their own data using data dictionaries and common standards. The sessions will cover topics such as exploratory data analysis, data validation, visualization, and more advanced topics like visibility analysis for point-to-point connectivity and fiber path analysis. The training will involve practical sessions where participants will gain hands-on experience using QGIS and Jupyter Notebooks, working through real-life case studies related to school connectivity.  

## Data

This course uses a case study of school connectivity in **Windhoek**, the capital of Namibia. While you'll learn to collect and process this data during the training, we provide pre-processed datasets at different stages to help you follow along.

### Data Repository

All training data is available in [this Google Drive folder](https://drive.google.com/drive/folders/1ANcLWuLDko8nnKuwaYU1S3QH8I8PIwT6?usp=drive_link), organized into the following subfolders:

- **raw/**: Original data as downloaded from various sources, before any processing
- **standardized/**: Cleaned and formatted data following ITU standards and data dictionaries, ready for analysis 
- **outputs/**: Results from different analyses (proximity, coverage, demand, etc.)
- **raster/**: Geographic raster files for elevation and population density

[![windhoek-schools.png](https://i.postimg.cc/rwnjc01M/windhoek-schools.png)](https://postimg.cc/68ZnfQbm)

_Figure: Query OpenStreetMaps using Overpass API_


### Data Sources

| Dataset | Source |
|---------|--------|
| School locations | OpenStreetMap |
| Cell sites | OpenCellID |
| Road network | OpenStreetMap |
| Fiber/transmission nodes | Ookla Speedtest |
| 4G mobile coverage | Operator data |
| Population density | WorldPop |
| Elevation data | SRTM/NASA |

Each source has been chosen to provide reliable, up-to-date information while being representative of data you might use in real-world connectivity planning projects.

## Training agenda

- **Day 1: Fundamentals of Geospatial Analysis**
   - **ICT Infrastructure Business Planning** [🔗](https://docs.google.com/presentation/d/1f5VOf5LS_9r4xHv2d1eLAV5VT_Zjmici/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Learn about business planning tools to evaluate the commercial viability of an ICT infrastructure project. This module shows how GIS tools are useful to extract the information that allows to compute the revenues and costs associated with a product.
   - **Geospatial Data Types** [🔗](https://docs.google.com/presentation/d/1zyqroBHlMC82NxhtD_vULcTDBKgY_mtL/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Master the fundamentals of vector, raster, and tabular data types, and understand when to use each format.
   - **Projections and Coordinate Systems** [🔗](https://docs.google.com/presentation/d/13s4Go1vj12nkUcNlgdOyqNUccCQj4ndU/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Learn how to work with different map projections and coordinate systems to ensure accurate spatial analysis.
   - **Telecommunications Open Data** [🔗](https://docs.google.com/presentation/d/1f9VRvwjXD3T4FVj_4TCxqGx4HlssLx4B/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Discover various telecommunications data sources, their characteristics, and learn to evaluate their advantages and limitations.
   - **Introduction to QGIS** [🔗](https://docs.google.com/presentation/d/1ZtxdFYOMHoRuo_l8w8xmG0_oMLKlsCHg/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Get started with QGIS, a powerful open-source software for geospatial analysis that will be our main tool throughout the course.
   - **Practical Sessions**:
       - **Open Data Collection** [🔗](https://docs.google.com/presentation/d/16KXbnI65sTZx74jhlOMorm0QJ_-rSlVo/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true): Master the tools and techniques for gathering telecommunications data from key sources like OpenStreetMap, GIGA Maps, and OpenCellID using APIs and QGIS plugins.
       - **Data Standardization** [🔗](https://docs.google.com/presentation/d/1AHv691p_IuWAT5TDrbVikPmzmOiLe18P/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Learn to prepare and clean data according to ITU Data Dictionaries standards using QGIS and SQL, ensuring it's ready for analysis.
       - **Proximity Analysis** [🔗](https://docs.google.com/presentation/d/16JQgci4pFSOHhEzrCYD3plY3TsCUnDZh/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true): Calculate distances between Points of Interest and existing infrastructure to help prioritize locations for infrastructure expansion and optimize deployment strategies. Creates graduated symbol maps showing distances to nearest infrastructure.
       - **Coverage Analysis** [🔗](https://docs.google.com/presentation/d/1Lxa-wgrB3bGAY7g4y4iU4_aodZs3w_Fv/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true): Map and analyze the geographic reach of existing mobile networks to identify areas with limited or no coverage. Generate coverage status maps by technology type (3G/4G/5G).
   - **Quizzes**:
       - Quiz on GIS Basics [🔗](https://www.mentimeter.com/app/presentation/alt6yhwbdsgabj236r5ajrq8j7ibanjv/edit?source=share-invite-modal)
       - Quiy on Open Data Sources in ICT [🔗](https://www.mentimeter.com/app/presentation/alss7u4hyjbx3iyrfjx16qu17xqxyse9/edit?source=share-invite-modal)
       - Quiz on Proximity, Coverage and Demand Analysis [🔗](https://www.mentimeter.com/app/presentation/algz675pgkbsctny2zm1xjftptvbwgr9/edit?source=share-invite-modal)

- **Day 2: Advanced Applications, Business Planning and Python Integration**
   - **Practical Sessions**:
       - **Demand Analysis** [🔗](https://docs.google.com/presentation/d/1crhy0LsVY5QjiccMAv1CYLPCKWVamA1g/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Calculate potential internet users and required throughput at each PoI using high-resolution population models that combine satellite imagery with census estimates. Includes analysis of population distribution within various buffer zones.
       - **Visibility Analysis** [🔗](https://docs.google.com/presentation/d/1SgWSPllPWiQHgm77HTHElC5BpR5iXX2z/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Evaluate line-of-sight between cell sites and points of interest, considering terrain and physical obstructions. Learn to assess feasibility of radio links and identify optimal locations for infrastructure deployment.
       - **Fiber Path Analysis** [🔗](https://docs.google.com/presentation/d/1NFMnqD7Nfcay0U1iW_IqmTzTa2sFpDP_/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Learn to design efficient fiber networks by leveraging existing infrastructure and optimizing routes for cost-effectiveness.
       - **Python & Google Colab Introduction** [🔗](https://docs.google.com/presentation/d/19Rq3JwB691SglRiOfPh-Y5yT_t6ebQ7x/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Learn about the Pros and Cons of using QGIS versus a programmatic approach using Python. Learn about using Google Colab to launch Jupyter notebooks, and discover the main Python libraries for working with geospatial data.
       - **Cost Analysis** [🔗](https://docs.google.com/presentation/d/1-V6xn-wx4_oeVG_MRE2WsE1hhID22T1L/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true) using Jupyter notebook `cost_modelling.ipynb` running on Google Colab. Learn to evaluate different technology options (fiber, cellular, point-to-point and satellite) and optimize deployment costs using microeconomic data. Calculate CapEx, OpEx, and potential revenues for different connectivity solutions.
       - **KeplerGL Visualization** [🔗](https://docs.google.com/presentation/d/12x5vK9G4nBbFDleSvsjrR3hQUgxKjGs3/edit?usp=sharing&ouid=110166480978407115454&rtpof=true&sd=true): Learn how to produce appealling visualizations using the online version of KeplerGL, a powerful suite of open-source visualization tools.
   - **Quizzes**:
       - Quiz on Fiber Path and Visibility [🔗](https://www.mentimeter.com/app/presentation/aljx818pzop4e9bcugepyk71dtgiwqgu/edit?source=share-invite-modal)

## Prerequisites

### For Google Colab Users
- A Google account (e.g., Gmail) to access Google Colab and training data
- No additional software installation required

### For Local Setup
- Python 3.11
- Jupyter Notebook/Lab
- QGIS version 3.34.9 'Prizren LTR' (Long-term release)
 - Available for Windows, Mac, and Linux
 - Required plugins:
   - Open Topography DEM Downloader
   - QNEAT3
   - Visibility Analysis
   - GRASS 8
   - QuickMapServices
   - QuickOSM

## Setup instructions

### To run notebooks locally

1. Clone the repository:

```bash
git clone https://github.com/FNS-Division/GIGA-mapping-training
cd GIGA-mapping-training
```

2. Create and activate the Conda environment:

```bash
conda env create -f environment.yml
conda activate inframaptraining
```

3. Launch Jupyter:

```bash
jupyter lab
```

### To run notebooks on Google Colab

All notebooks are created using Google Colab for easy accessibility. In order to run them on [Google Colab](https://colab.research.google.com/), you will need to sign in with a Google account. If you are unfamiliar with Google Colab, please watch this [introductory video](https://www.youtube.com/watch?v=inN8seMm7UI).

1. Navigate to each notebook in the repository
2. At the top of each notebook, click on the **Open in Colab** button.

<a href="https://colab.research.google.com/github/sg-peytrignet/algeria24-training/blob/main/3_fiber_modeling.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

## Contributing

Please submit a pull request to contribute to this repository.

## License

Please refer to our [license](LICENSE).

## Contact

For questions or support, please create an issue in this repository or get in touch at [fns@itu.int](fns@itu.int).
