# GIGA-mapping-training

Training materials for an ITU course provided as part of the following event focusing on network infrastructure analysis and planning:

[Infrastructure mapping for school connectivity](https://academy.itu.int/training-courses/full-catalogue/infrastructure-mapping-school-connectivity), Geneva – Switzerland, 27-28 February 2025

<a href="https://ibb.co/yW090yp"><img src="https://i.ibb.co/4PWqWT2/windhoek-fiber.png" alt="windhoek-fiber" border="0"></a>

_Figure: Fiber path simulation in Windhoek, Namibia_

## Table of Contents

1. [Overview](#overview)
2. [Repository Structure](#repository-structure)
3. [Pre-requisites](#pre-requisites)
4. [Setup Instructions](#setup-instructions)
   - [Run Locally](#to-run-notebooks-locally)
   - [Run on Google Colab](#to-run-notebooks-on-google-colab)
5. [Usage Notes](#usage-notes)
6. [Contributing](#contributing)
7. [Acknowledgements](#acknowledgements)
8. [Contact](#contact)
9. [License](#license)

## Overview

This repository contains links to course slides hosted on a [Google Drive folder](https://drive.google.com/drive/folders/1-4AfC8c9T6JMUHEtFtCyKlLG3kGGERIL?usp=sharing), Jupyter notebooks and supporting materials for 2-day course on infrastructure mapping and analysis.

The course covers an introduction to GIS systems, data standardization, visualization, coverage analysis, fiber path modeling, and cost estimation.

## Training agenda

- **Slides:**
    - **Day 1: Introduction to geospatial data:** Covers the basics of GIS, Python-based geospatial data processing, and visualizations with KeplerGL.
        - [Introduction to Python and Google Colab](https://docs.google.com/presentation/d/1tEIVCvb1jg2W_CS8A1l6VXxEQgrczHV8/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Visualization with KeplerGL](https://docs.google.com/presentation/d/1_HZsWGcwOvX-Pa4kFjlvza4m0K311EP4/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Introduction to QGIS](https://docs.google.com/presentation/d/15INri2v9S72rlaeca5pQ1jSz4aRHX8na/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Introduction to working with geospatial data](https://docs.google.com/presentation/d/1xRUdM9k82wZLib_vweeiH3mF4XSlKmQp/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Projections and coordinate reference systems](https://docs.google.com/presentation/d/1PO7kVzpYnWp0P-H-1veo10Peu_fwoTwH/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Open geospatial data in telecommunications](https://docs.google.com/presentation/d/1nHZnf2F1kje_mxuW1e9UV-G02RBAb79Z/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [ICT data collection and processing](https://docs.google.com/presentation/d/1JBSYWGjTfd06zPZbCO7ZxUogQ3Y1F82C/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Quiz](https://www.mentimeter.com/app/presentation/alnt3kcapjfsshbb5vghyhfkdhv4jt7d/edit?source=share-invite-modal)
    - **Day 2: Infrastructure analysis tools:** Explores advanced concepts such as network modeling, demand analysis, and cost estimation.
        - [Network analysis](https://docs.google.com/presentation/d/1XAxjJScfZkU8KMzbHWv53H_FonTibvBu/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Demand analysis](https://docs.google.com/presentation/d/1f3eJDYS5WBYDcZyzOMgHA8HwQymqxkJH/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [ICT infrastructure business planning](https://docs.google.com/presentation/d/1s4rMN5QZQv5r3q9A2nSzQgWoARpcrp8_/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Fiber path analysis](https://docs.google.com/presentation/d/1t1SSuF3vlDaIvWTYrhOB3pWFfSYqPPRo/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Visibility analysis](https://docs.google.com/presentation/d/17q7peog0sNe90KYfLtQJmFi3YP-2iCu0/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Cost analysis](https://docs.google.com/presentation/d/1JvHnThJJXZyLwUU8cfL-0dFC3QUgLBVY/edit?usp=drive_link&ouid=110166480978407115454&rtpof=true&sd=true)
        - [Quiz](https://www.mentimeter.com/app/presentation/alp66s3gqeyxokxjepj4gdno2duwmc38/edit?source=share-invite-modal)
- **Jupyter Notebooks:**
    - [`0_eda_standardization.ipynb`](0_eda_standardization.ipynb): Data exploration and standardization procedures
    - [`1_proximity_coverage_demand.ipynb`](1_proximity_coverage_demand.ipynb): Analysis of coverage proximity and demand mapping
    - [`2_visibility_analysis.ipynb`](2_visibility_analysis.ipynb): Visibility and line-of-sight analysis for network planning
    - [`3_fiber_modeling.ipynb`](3_fiber_modeling.ipynb): Fiber network modeling and optimization
    - [`4_cost_modelling.ipynb`](4_cost_modelling.ipynb): Cost estimation and financial modeling

## Pre-requisites

To run the Jupyter notebooks on **Google Colab**, you'll need:
- A Google account (e.g. a Gmail account).

To run these notebooks **locally**, you'll need:

- Python 3.9
- Jupyter Notebook/Lab

## Setup instructions

### To run notebooks locally

1. Clone the repository:

```bash
git clone https://github.com/sg-peytrignet/algeria24-training.git
cd algeria24-training
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

## Usage notes

Follow the notebooks in numerical order for the best learning experience.

## Contributing

Please submit a pull request to contribute to this repository.

## License

Please refer to our [license](LICENSE).

## Contact

For questions or support, please create an issue in this repository or get in touch at fns@itu.int.

## Acknowledgements

We would like to thank South Korea's Ministry of Science and ICT for their support.

![sponsor](https://i.ibb.co/tXQqP2S/image.jpg)
