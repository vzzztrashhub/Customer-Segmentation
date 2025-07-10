# Customer Segmentation using Machine Learning

This project focuses on segmenting customers based on their purchasing behavior and personal information. It uses clustering and classification models to help businesses understand their customer base for targeted marketing.

## Problem Statement

Retailers and service providers often need to group customers based on behavior to offer personalized experiences. In this project, machine learning techniques are used to identify patterns and segment customers effectively.

## Solution Overview

- Performed exploratory data analysis and preprocessing.
- Applied **K-Means Clustering** to group customers into clusters.
- Used **Logistic Regression** to classify new customers into the right cluster.
- Built an end-to-end pipeline for data ingestion, transformation, training, and prediction.

## Dataset

The dataset contains customer demographic and purchasing data such as:
- Age
- Income
- Spending score
- Marital status
- Campaign responses

## Models Used

- **K-Means Clustering** – for customer segmentation  
- **Logistic Regression** – to predict cluster group of new customers  
- **GridSearchCV** – for hyperparameter tuning

## Tech Stack

1. Python
2. FastAPI
3. Machine learning algorithms
4. Docker
5. MongoDB

## Infrastructure required

1. AWS S3
2. Azure
3. Github Actions

## How to Run

Before running this project make sure you have MongoDB Atlas account and you have the shipping dataset into it.

Step 1. Cloning the repository.

```

git clone https://github.com/Machine-Learning-01/Customer_segmentation.git

```

Step 2. Create a conda environment.

```

conda create --prefix venv python=3.7 -y

```

```

conda activate venv/

```

Step 3. Install the requirements

```

pip install -r requirements.txt

```

Step 4. Export the environment variable

```bash

export AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID>


export AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY>


export AWS_DEFAULT_REGION=<AWS_DEFAULT_REGION>


export MONGODB_URL= <MONGODB_URL>


```

Step 5. Run the application server

```

python app.py

```

Step 6. Train application

```bash

http://localhost:5000/train

```

Step 7. Prediction application

```bash

http://localhost:5000/predict

```

## Run locally

1. Check if the Dockerfile is available in the project directory
2. Build the Docker image
3. Run the Docker image

## Key Features

- End-to-end ML pipeline from preprocessing to model deployment
- FastAPI integration for prediction as a service
- Docker support for easy deployment
- MongoDB connectivity for production-level storage

## Conclusion

This project demonstrates a complete ML lifecycle for customer personality segmentation. It can help businesses improve marketing strategy, resource allocation, and customer experience.
