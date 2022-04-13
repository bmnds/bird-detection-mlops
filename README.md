# bird-detection-mlops
MLOps project to detect the bird species from its image. Model trained on Kaggle. Backend hosted on GCP. Frontend thanks to Streamlit.

## Submodules
This is an umbrella project to link together all deliverables of this solution, which are:
* _bird-detection-model_ the heart of the solution, a machine learning model built with Python & Jupyter Notebooks and trained using Kaggle resources, it is capable of predicting the species of a bird out of its image;
* _bird-detection-api_ is the brain of the solution, responsible for publishing the model to the world, built using Python & Flask and hosted on Google Cloud Platform;
* _bird-detection-web_ is the pretty face of the solution, a prototype built with and hosted by Streamlit to let end users play around with the model and check its capabilities via any browser Mobile or Desktop.

## Architecture
The following picture depicts how each submodule interconnects with each other, plus, how the MLOps pipeline is configured to fetch the latest changes directly from GitHub and make it all the way to production.

![Arquitetura](architecture.png?raw=true)