## Predicting Transit Ridership Using Satellite Imagery and GTFS Data: A Deep Learning Approach for Sustainable Mobility in Philadelphia ##

Regy Septian & Xiaxin Tang – Master of City Planning 2025 MUSA 695-AI for Urban Sustainabilit

### Introduction and Motivation
**Transit ridership** is a key metric for understanding the performance and equity of public transportation systems. Traditional ridership studies rely on survey data or detailed operations datasets, which are not always available in every region. This project explores whether satellite imagery alone can be used to predict public transit ridership levels at bus stops, using machine learning.

By linking built environment features (as seen from above) with ridership patterns, we aim to train a convolutional neural network (CNN) to identify visual indicators that correlate with stop-level ridership. This approach could help transit agencies and urban planners analyze demand in data-scarce areas or assess where ridership potential is being underutilized.

The key question this project explores is: **Can a CNN model learn to predict public transit ridership from satellite imagery, and identify spatial patterns associated with high or low demand?**

If successful, this model could help planners and researchers quickly assess accessibility in data-scarce regions by analyzing only image data and supporting transportation equity, transit-oriented development, and sustainability planning efforts.

### Data Sources
**1. GTFS (SEPTA)**
GTFS (General Transit Feed Specification) is a standardized format for organizing public transit schedules and route information, enabling easy data exchange between systems and powering trip-planning apps like Google Maps. More info can be found at gtfs.org.

Although GTFS was not used directly in class, it offers significant value for geospatial analysis — especially in the U.S. context. Over 2,500 transit agencies worldwide publish GTFS feeds, and as of Fall 2023, it has become a required reporting format for the National Transit Database administered by the Federal Transit Administration. This widespread adoption makes GTFS a robust, scalable tool for analyzing transit accessibility.

For this project, I will use the SEPTA GTFS feed (available here, last updated March 2025) to compute accessibility scores for locations across Philadelphia. These scores will serve as ground-truth labels for training the CNN model.
**2. NAIP Imagery**
NAIP image tiles over Philadelphia will be used as the input data for the CNN. Each image patch will be labeled based on its transit accessibility class (e.g., high, medium, low) derived from GTFS.

### Result ###
A CNN model with a test accuracy of 80.45% that can be used to predict bus ridership based on landuse imageries.
