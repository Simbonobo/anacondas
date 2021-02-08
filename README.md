# anacondas
Team assignment of team "anacondas" as part of the Advanced Analytics course at university of cologne. Examined cities: Bonn, Essen

![Anacondas](https://miro.medium.com/max/1000/1*h1h6j08kIHv3ywN3MCfKLg.jpeg)


## Setup

As we notices some issues with changing package versions, please set up environment as followed:

Create a conda environment with the packages noted in our environment.yaml:

    create --name  [your_environment] --file environment.yaml

Activate your newly created environment:

    conda activate [your_environment]
    
Afterwards use pip to install all packages stated in our requirement.txt:

    pip install -r requirements.txt


XGboost somtimes runs into problems with macOS. If you run into these problems install xgboost with conda 

    conda install -c conda-forge xgboost

or install the libmop library as suggested in the error message:

    brew install libomp

    
## Notebook descriptions

### Preprocessing
In this notebook the data sets is generated, loaded from the given '.csv' files and using nextbike's API. Afterwards the data sets are formatted, cleaned and saved to  '.pickle' files.

### Weather
In this notebook the weather data for Bonn and Essen is loaded from german weather service website. Afterwards the data is formatted, cleaned, missing values are added and saved to '.pickle' files. Furthermore weather data correlations are calculated at the end of the notebook.

### KPI
In this notebook the preprocessed data sets are applied to create five different key performance indicators to develop a detailed understanding for nexbikes business.

### Clustering
In this notebook the preprocessed data sets are applied to identify different types of customer groups, clustered by trip duration and trip distance depending on the time of day.

### Model
In this notebook the preprocessed data sets (cities and weather) are used to predict the daily rental demand with the help of predictive analyses.

