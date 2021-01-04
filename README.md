# AirBnb Data Analysis

## Table of contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, Acknowledgement](#others)

<br>

## Installation

<a id="installation"></a>
The code here basically run on the Anaconda distribution of Python (version 3.\*).

GeoPandas packages must be downloaded to fully explore the project work. The libraries include geopandas, descartes, shapely, which are additionally installed on an Anaconda environment.

To install the package with conda run the below on the command line.

-   **Geopandas:** conda install -c conda-forge geopandas
-   **Descartes:** conda install -c conda-forge descartes
-   **Shapely:** conda install -c conda-forge shapely

<br>

## Debugging

When trying to import the GeoPandas libraries on the Jupyter Notebook, I faced
ModuleNotFoundError. I researched online and found some breakthroughts that work for me, which are listed as following:

1. A documentation that explains the potential causes at the link [here](<(https://jupyter-notebook.readthedocs.io/en/stable/troubleshooting.html)>)

2. [Actual commands that helped for me](https://stackoverflow.com/questions/28831854/how-do-i-add-python3-kernel-to-jupyter-ipython) as below. Copy and paste on your command line interface :

    python3 -m pip install ipykernel<br>
    python3 -m ipykernel install --user

<br>

## Motivation

<a id="motivation"></a>
For this project, I used 2016 Airbnb data for two U.S. cities, Seattle and Boston, to better understand:

-   How has occupancy rate and average room rate evolved every month in 2016? Is there a better metric to use when evaluating the overall Airbnb rental performance?

-   How does the supply side look? How has new listings grown over time? What are the general characteristics of hostings, in terms of types of host, property, room? How much is Airbnb rental price?

-   Does the rental price vary in different neighborhoods? Is there a better graphical way to represent the data?

<br>

## Files

<a id="files"></a>
The main notebook is named as `analysis.ipynb` to show codes related to the project questions.

Two folders are to contain data used for the analysis.

-   `data` : two zip files for Seattle and Boston Airbnb data, of which three csv files can be extracted respectively.
-   `geodata` : geospatial data files for the two U.S. cities - only .shp files are used ([shapefile](https://en.wikipedia.org/wiki/Shapefile))

Additionally, I trialed a geographically analysis for the first time and practiced on `geopandas_exercise.ipynb` after a tuturial provided online (the tutorial can be found [here](#geopandas))

<br>

## Results

<a id="results"></a>

The results are discussed at my personal post [here](#).

<br>

## Licensing, Authors, Acknowledgement

<a id="others"></a>

The project is part of [Udacity's Data Scientist Nano Degree](https://www.udacity.com/course/data-scientist-nanodegree--nd025) program. It is intended to review CRISP-DM(Cross-Idustry Standard Process for Data Mining) and apply concepts to the real world problem.

The datasets are available at the Kaggle website where the licensing for the data and other information are also described.

> [Link to the Seattle Airbnb data](https://www.kaggle.com/airbnb/seattle/data) <br> [Link to the Boston Airbnb data](https://www.kaggle.com/airbnb/boston)

Also, some geographical data are used to help my analysis, and openly available at the links below:

> [Seattle GeoData](https://data-seattlecitygis.opendata.arcgis.com/datasets/city-clerk-neighborhoods) <br> [Boston Neighborhoods](https://bostonopendata-boston.opendata.arcgis.com/datasets/3525b0ee6e6b427f9aab5d0a1d0a1a28_0)

<a id="geopandas"></a>
Lastly, I got a lot of helps from a `GeoPandas` tutorial post by Ryan Stewart at the link [here](https://towardsdatascience.com/geopandas-101-plot-any-data-with-a-latitude-and-longitude-on-a-map-98e01944b972).
