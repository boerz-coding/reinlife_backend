
# ReinLife_Backend
Backend code for ReinLife app (mHealth platform).

ReinLife is a machine learning-based open source mobile health (mHealth) platform. ReinLife is designed for ML and clinical researchers to design and implement cross-utting skill learning experiments. ReinLife appears as a mobile app in the frontend, and in the backend, it provides a set of Python APIs that allow users to set up experiments, collect information from users, and send them personalized interventions to help them make progresses.   [This](https://tbd) is a manuscript introducing the platform in more details.

We are using Google Firebase service and Python to build our backend. This document provides instruction on how to run the backend. 
 
The frontend is written in flutter and can be found at [reinlife_flutter](https://github.com/ReinLife-AC297r/reinlife_flutter).

# Current Workflow
## Creating a new Firebase project

To manage their own backend, the researchers are supposed to create their own Firebase project.

## Running python code
1. Recreate python/anaconda environment using environment.yml
2. Researchers can look at `example_researcher_defined_code.ipynb` which is a jupyter notebook that contains the example code of of the API should be used. The APIs are in the module `ReinLifeResearcher.py`



## Environment Configuration
<!--
### Create Envionement
 conda activate relearnlife
 conda install flask requests
### Save Env
 conda env export > environment.yml)
-->
### Recreate Env
I am using anaconda to create the environment. Here are the steps to repeat the envionment.
```
conda env create -f environment.yml
conda activate reinlife
```
## files
`ReinLifeResearcher.py` is the module that contains APIs for researchers to use

`server2firestore.py` is a module that contains helper functions to communcate with the firestore. We do not currently have an extra server layer in our current implementation although it is named as "server"2firstore.

`example_researcher_defined_code.ipynb` is a jupyter notebook that contains the example code of of the API should be used.

