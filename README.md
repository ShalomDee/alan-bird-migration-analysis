# Investigating Artificial Light at Night and Bird Migration

This project examines how artificial illumination at night influences nocturnal bird migration across Vermont and New Jersey. The work combines remote sensing, ecological data analysis, and predictive modeling, completed within the AI4ALL Ignite accelerator, where our group applied statistical reasoning, machine learning, and data engineering practices to study light pollution and bird movement dynamics.

## Problem Statement

Artificial illumination is increasing globally, and its ecological effects are especially pronounced for nocturnal migrants that depend on the night sky for navigation. Light exposure can disrupt orientation, alter flight behavior, and increase collision risks in regions near intense radiance. Vermont offers an environment with relatively low illumination that provides a strong reference point, while New Jersey represents a region with substantial artificial lighting. The project evaluates how varying light conditions relate to migration intensity, altitude, speed, and directional patterns. This work supports conservation efforts, policy conversations, and long term planning for bird safe initiatives.

## Key Results

1. Constructed a complete data pipeline integrating BirdCast migration metrics with NASA and NOAA VIIRS nightly radiance products.
2. Generated a merged dataset that includes migration intensity, altitude, speed, directional movement, corrected radiance values, lunar conditions, cloud indicators, snow presence, and temporal features.
3. Identified notable patterns in peak migration nights, showing meaningful contrasts between low illumination and high illumination regions.
4. Trained statistical models and machine learning regressors to evaluate relationships between migration indicators and artificial illumination, cloud cover, lunar brightness, and seasonal timing.
5. Produced visual summaries that contextualize how light intensity varies across the study areas and how migration activity responds to these patterns.

## Methodologies 

Data preparation involved collecting BirdCast migration observations through lawful scraping methods and downloading nightly illumination products from NASA and NOAA VIIRS sources. The team created Colab based scripts for data extraction, cleaning, and transformation. Processed radiance layers were merged with migration metrics using consistent temporal alignment and quality filters.

Analytical methods included linear regression, generalized additive modeling, random forest regression, and gradient boosting models. These approaches captured both interpretable associations and more complex interactions among predictors. The team examined feature contributions, temporal trends, and cross regional contrasts between Vermont and New Jersey. The analysis supports ecological interpretation by connecting patterns in radiance measurements with measurable changes in migration behavior.


## Data Sources 

- BirdCast Migration Dashboard, Cornell Lab of Ornithology: [Link to BirdCast](https://dashboard.birdcast.info/)
- NASA VIIRS VNP46A2 daily radiance: [Link to VNP46A2 Data](https://developers.google.com/earth-engine/datasets/catalog/NASA_VIIRS_002_VNP46A2)
- NOAA VIIRS VNP46A1 radiance and cloud condition indicators: [Link to VNP46A1 Data](https://developers.google.com/earth-engine/datasets/catalog/NOAA_VIIRS_001_VNP46A1)
- Presentation figures and data summaries from the Night Bird Migration Group Project Presentation

## Technologies Used 

- Python
- pandas
- NumPy
- scikit learn
- Google Colab
- Jupyter
- Web scraping tools for BirdCast data retrieval
- NASA and NOAA VIIRS remote sensing products processed via Earth Engine workflows


## Authors

This project was completed by:
- Shalom Donga ([LinkedIn](https://www.linkedin.com/in/shalom-donga))
- Tatenda Kasirori ([LinkedIn](https://www.linkedin.com/in/tatenda-kasirori))
- Kambili Nwankwo ([LinkedIn](https://www.linkedin.com/in/kambili-nwankwo))
