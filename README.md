[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Ganiyat-dev/Operationalize-ML-Microservice/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Ganiyat-dev/Operationalize-ML-Microservice/tree/main)

# Project Summary

## **operationalize production microservices**
This project operationalize a Machine Learning Microservice API, using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. 

Given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing).

This project operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.


### Project Tasks

The following was carried out:
* Testing the project code using linting
* Complete a Dockerfile to containerize this application
* Deploy the containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that the code has been tested

# Running the Python scripts and web app
---

## Setup the Environment (using AWS cloud 9)

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv

python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

* prediction outputs

![Screenshot from 2022-09-03 09-38-36](https://user-images.githubusercontent.com/60348108/188265716-925fdc53-de3a-4f6d-9909-670edea71f3f.png)

![Screenshot from 2022-09-03 07-25-22](https://user-images.githubusercontent.com/60348108/188265732-934e4930-03f4-4cac-bda3-54007963f6e0.png)





