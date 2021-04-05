# suma-hakaton-2021


Suma hackathon 2021 competition project.


<h1>About</h1>


Our final product for hackathon competition was an android app that would inform people about air pollution in Belgrade.
It does so by using an API to lookup meteorological data for the current day.

After collecting meteorological data and processing it to be in the appropriate form, the trained model is used to predict values of 6 different air pollutants.
The air quality index (AQI) is calculated from air pollutants prediction in order to have one value describing how much the air is polluted.

The prediction model was trained using meteorological data and pollution data for Belgrade. 
Both datasets required heavy preprocessing including filling missing values by interpolation,
predicting missing values with models trained on values that were already there, 
eliminating fully correlated attributes, irrelevant attributes, and attributes that were not measured enough times.


<h1>Files</h1>


Android app: `PolluteOrSalute.zip`


Trained model for predicting pollutants saved as state dictionary: `modelPollution_12.58`


Model architecture and training: `pollution_model.ipynb`
Model evaluation and AQI(air quality index) calculation based on predictions: `pollution_model_evaluation.ipynb`


AQI calculation: `calculate_air_quality_index.ipynb`


Meteo data after preprocessing: `podaci_final_VV_popunjeno_bezH.csv`
Pollution data after preprocessing: `pollutionData.csv`


Models used for predicting missing values in meteo dataset: `model_fill_Ff.ipynb` and `model_fill_VV.ipynb`
Filling missing values: `fill_VV.ipynb` and `fill_Ff.ipynb`


Other notebooks were used for preprocessing datasets.


<h1>Collaborators</h1>

Nikola Andric Mitrovic: https://github.com/andricmitrovic

Mihailo Jovanovic: https://github.com/oliahim98

Marija Eric: https://github.com/MarijaEric

Bozidar Mitrovic: https://github.com/AizenAngel

All commits were submitted by Bozidar Mitrovic while working on the project.
