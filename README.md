# Student Exam Performance Indicator

Welcome to the **Student Exam Performance Indicator** web application! This system is designed to analyze and predict students' academic performance based on various input factors, primarily focusing on predicting a student's math score.

## Project Overview

The Student Exam Performance Indicator utilizes machine learning techniques to predict students' math scores based on their personal and academic data. The system takes into account factors such as gender, parental education level, test preparation status, and scores in reading and writing.

The project is deployed on Azure, with containerized management using Azure Container Registry (ACR). The model was trained using the **Students Performance in Exams** dataset from Kaggle.

## Dataset Details

The dataset used in this project contains the following features for prediction:

- **Gender**: Indicates the gender of the student (e.g., male or female).
- **Race/Ethnicity**: Categorizes students based on race/ethnicity (e.g., group A, group B, etc.).
- **Parental Level of Education**: Represents the highest level of education completed by the student's parent or guardian.
- **Lunch**: Indicates the type of lunch the student receives (e.g., standard or free/reduced).
- **Test Preparation Course**: Specifies whether the student completed a test preparation course (completed or none).
- **Reading Score**: The score obtained by the student in the reading test.
- **Writing Score**: The score obtained by the student in the writing test.


## Key Features

Our web application provides:

- An intuitive interface for entering student details.
- Real-time predictions of math scores based on input data.
- A user-friendly and effective experience for predicting student performance.

## Deployment Details

This project is deployed on Azure. The deployment leverages Azure Container Registry (ACR) for containerized management of the application.

### How It Works:
- The machine learning model was trained using the above features, and predictions are made based on student input on the prediction page.
- The app provides a prediction of the student's math score once all required details are entered.

## Try It Out

- **Home**: Visit the home page to get an overview of the project.
- **Prediction Page**: Head to the prediction page to enter student details and get predictions for the math score.

## Explore the Source Code

You can find the source code and contribute to the project on our [GitHub repository](https://github.com/AnimeshBasak-14/StudentPerformancewithAzureDeployment).

## How to Set Up Locally

### Prerequisites:
- Python 3.x
- Flask
- Docker (for containerized deployment)
- Azure (for managing Azure resources)


## Installation Guide

# Student Exam Performance Indicator

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AnimeshBasak-14/StudentPerformancewithAzureDeployment.git
   cd StudentPerformancewithAzureDeployment


   docker login myregistername.azurecr.io

   use username and password to login

   docker push myregistername.azurecr.io/application_name:version 

2. Set up a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use venv\Scripts\activate
   pip install -r requirements.txt

3. Set up MS Azure Container Registries:

After creating the container, you will see Access keys.
Save the login server, username, and password.

4. Create Docker Image:
      ```bash
      docker build -t myregistername.azurecr.io/application_name:version .
      docker login myregistername.azurecr.io
      Use the saved username and password to log in.

5. Set up Web App in Azure: Complete the necessary setup. After completion, go to the deployment center and connect to your GitHub account. This will automatically create .github/workflows/main_myregistername.yml in your GitHub repository.

6. Go to GitHub Actions: The build and deploy process will happen automatically. You can access your web app through the link provided in the default domain in the Web App resource.


