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


XGboost somtimes runs into problems with mscOS. If you run into these problems install xgboost with conda 

    conda install -c conda-forge xgboost

or install the libmop library as suggested in the error message:

    brew install libomp