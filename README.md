# Course-Exploring_SageMaker
Udacity's Deep Learning Nanodegree Course 6 - Deploy a Model

1) Use the main.sh script to deploy the infrastructure

    a) Deploy Network

    b) Deploy Notebook

    c) Deploy IAM

    d) Deploy Lambda

2) Once the Notebook Instance is finished deploying, go into the Notebook Instance

    a) Navigate to Tutorial > Web App

3) Execute all the cells from 1 to 30

    a) last cell to execute: `xgb_predictor = xgb.deploy(initial_instance_count = 1, instance_type = 'ml.m4.xlarge')`

4) Update the Lamda function's two lines with the info from the notebook

    a) vocab = `print(str(vocabulary))`

    b) EndpointName = `xgb_predictor.endpoint`

5) Go back to the main Jupyter folder and download index.html

6) Modify the action to be the AWS API Gateway URL

    a) action="**REPLACE WITH PUBLIC API URL**"

