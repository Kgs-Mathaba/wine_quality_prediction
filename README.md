# Wine Quality Prediction Project

## Project Overview 📚

Welcome to the Wine Quality Prediction project! In this exploration of oenology, we delved into the fascinating world of wine quality assessment. The primary goal of this project was to develop an end-to-end machine learning solution capable of predicting the quality of wines based on various attributes.

### Project Mission 🚀

Armed with a comprehensive dataset encompassing diverse attributes of different wines, we embarked on a mission to build a robust predictive model. The objective was to create a model that could assess wine quality with remarkable accuracy, providing valuable insights into the intricate world of oenology.

## Key Features 🌟

- **Machine Learning Modeling:** Leveraged state-of-the-art machine learning algorithms to create a predictive model.
  
- **Data Exploration:** Explored and analyzed the dataset to understand the relationships between different attributes and the overall quality of wines.

- **Feature Engineering:** Engineered relevant features to enhance the model's predictive capabilities.

- **Evaluation and Validation:** Rigorously evaluated the model's performance using appropriate metrics and validated its effectiveness through cross-validation.

## Project Structure 📂

The repository is organized into the following key directories:

- **data:** Contains the dataset used for training and testing the machine learning model.

- **notebooks:** Jupyter notebooks detailing the step-by-step process of data exploration, feature engineering, and model training.

- **scripts:** Includes any scripts or utility files used in the project.

- **models:** Stores the trained machine learning model for deployment.

## Getting Started 🚦

Follow these steps to get started with the project:

1. Clone the repository: `git clone https://github.com/your-username/wine-quality-prediction.git`
2. Navigate to the project directory: `cd wine-quality-prediction`
3. Explore the Jupyter notebooks in the `notebooks` directory to understand the project workflow.
4. Check out the `models` directory for the trained machine learning model.

## How to Contribute 🤝

We welcome contributions and feedback! If you would like to contribute to the project, please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`.
3. Make your changes and commit them: `git commit -m 'Add new feature'`.
4. Push to the branch: `git push origin feature-branch`.
5. Submit a pull request.

## License 📜

This project is licensed under the [MIT License](LICENSE.md) - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments 👏

Special thanks to the oenology community and the contributors who helped make this project possible!

Happy wine predicting! 🍷✨



## Workflows

1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline 
8. Update the main.py
9. Update the app.py



# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/entbappy/End-to-end-Machine-Learning-Project-with-MLflow
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n mlproj python=3.8 -y
```

```bash
conda activate mlproj
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```



## MLflow

[Documentation](https://mlflow.org/docs/latest/index.html)


##### cmd
- mlflow ui

### dagshub
[dagshub](https://dagshub.com/)

MLFLOW_TRACKING_URI=https://dagshub.com/entbappy/End-to-end-Machine-Learning-Project-with-MLflow.mlflow \
MLFLOW_TRACKING_USERNAME=entbappy \
MLFLOW_TRACKING_PASSWORD=6824692c47a369aa6f9eac5b10041d5c8edbcef0 \
python script.py

Run this to export as env variables:

```bash

export MLFLOW_TRACKING_URI=https://dagshub.com/entbappy/End-to-end-Machine-Learning-Project-with-MLflow.mlflow

export MLFLOW_TRACKING_USERNAME=entbappy 

export MLFLOW_TRACKING_PASSWORD=6824692c47a369aa6f9eac5b10041d5c8edbcef0

```



# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: 566373416292.dkr.ecr.ap-south-1.amazonaws.com/mlproj

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optinal

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app




## About MLflow 
MLflow

 - Its Production Grade
 - Trace all of your expriements
 - Logging & tagging your model


