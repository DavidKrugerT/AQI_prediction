# Air Quality Prediction
Authors: Anton Zam & David Krüger.
## Feature pipeline
In the feature pipeline we retreived the data from two different API's; [Air Quality Index - aqicn.org](https://aqicn.org/data-platform/token-confirm/1a6ac705-bf60-4e38-b11d-be24807c2edb)
& wheather data [Historical Weather API - open-meteo.com](https://open-meteo.com/en/docs/historical-weather-api). We uploaded two feature groups on [hopsworks](https://www.hopsworks.ai/).  
## Feature views and training pipeline
For this part we combined the two feature groups into one feature view in order to assemble the traning data. 
## Training pipeline
first step was to clean and drop unnecessary featues. this data was then used to train three different models; Gradient boosting regressor, random forest and, a neural network which we ran some hyperparameter tuning on with bayesian optimization. 
## Huggingface
The model was then put on Huggingface where we predict 7 days of AQI. 
