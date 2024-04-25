# The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques
Due to rapid growth in field of cashless or digital  transactions, credit cards are widely used in all  around the world. Credit cards providers are  issuing thousands of cards to their customers.  Providers have to ensure all the credit card users  should be genuine and real. Any mistake in issuing  a card can be reason of financial crises.  
In this section we overview our selected method for engineering our solution. CRISP-DM stands for Cross-Industry Standard Process for Data Mining. It is an open standard guide that describes common approaches that are used by data mining experts. CRISP-DM includes descriptions of the typical phases of a project, including tasks details and provides an overview of the data mining lifecycle. The lifecycle model consists of six phases with arrows indicating the most important and frequent dependencies between phases. The sequence of the phases is not strict. In fact, most projects move back and forth between phases as necessary. It starts with business understanding, and then moves to data understanding, data preparation, modelling, evaluation, and deployment. The CRISP-DM model is flexible and can be customized easily.
key Features:-
Buissness Understanding
Tasks:

1.Determine business objectives

2.Assess situation

3.Determine data mining goals

4.Produce project plan
Data Understanding
 Tasks:

1.Collect data

2.Describe data

3.Explore data    
Data Preparation
Tasks:

1.Data selection

2.Data preprocessing

3.Feature engineering

4.Dimensionality reduction

        Steps:

        Data cleaning

        Data integration

        Data sampling

        Data dimensionality reduction

        Data formatting

        Data transformation

        Scaling

        Aggregation

        Decomposition
Data Modeling :
Modeling is the part of the Cross-Industry Standard Process for Data Mining (CRISP-DM) process model that i like best. Our data is already in good shape, and now we can search for useful patterns in our data.

Tasks:

1. Select modeling technique Select technique

2. Generate test design

3. Build model

4. Assess model
Data Evaluation :
Tasks:

1.Evaluate Result

2.Review Process

3.Determine next steps

Buissness Understanding
There may be two types of questions:

A.Technical Questions:

Can ML be a solution to the problem?

            Do we have THE data?
            Do we have all necessary related data?
            Is there enough amount of data to develop algorithm?
            Is data collected in the right way?
            Is data saved in the right format?
            Is the access to information guaranteed?
Can we satisfy all the Business Questions by means of ML?

B.Business Questions:

What are the organization's business goals?

            To reduce cost and increase revenue? 
            To increase efficiencies?
            To avoid risks? To improve quality?
Is it worth to develop ML?

            In short term? In long term?
            What are the success metrics?
            Can we handle the risk if the project is unsuccessful?
Do we have the resources?

            Do we have enough time to develop ML?
            Do we have a right talented team?
WE are provided a synthetic dataset for a mobile payments application. In this dataset, you are provided the sender and recipient of a transaction as well as whether transactions are tagged as fraud or not fraud. Your task is to build a fraud detection API that can be called to predict whether or not a transaction is fraudulent.

You are expected to build a REST API that predicts whether a given transaction is fraudulent or not. You are also to assume that the previous API calls are to be stored in order to engineer features relevant to finding fraud. The API calls will include the time step of the transaction, so you can assume that a transaction happens sequentially within the same time step. For example, if I make the following transactions in the same time step:

image.png

The first transaction is unlikely to be fraudulent, since anon is initiating a normal transfer. However, multiple successive transfers of the same amount in the same hour is potentially fraudulent, since anon’s account might have been taken over by a fraudster. On the first API call,your model is unlikely to classify the transaction as fraudulent. However, on the fifth call, it’s likely that it will be tagged as fraudulent. The REST API only has 1 endpoint /is-fraud that takes in a POST request:

The body is expected to receive the following fields(which are also the fields that can be found in your dataset: The following is a sample body when making a POST request to your

        {
    "step":1,
    "type":"PAYMENT",
    "amount":9839.64,
    "nameOrig":"C1231006815",
    "oldbalanceOrig":170136.0,
    "newbalanceOrig":160296.36,
    "nameDest":"M1979787155",
    "oldbalanceDest":0.0,
    "newbalanceDest":0.0
    }
Your API is expected to return a JSON object with a boolean field isFraud. You may find a sample response below:

{"isFraud": true}
summary: we are expecting the following:

Deployed REST API:
a. As mentioned above, we would need an API that takes in a POST request for the /is-fraud url and returns a prediction on whether or not a transaction is fraudulent.

b. Your REST API should be public for us to call the API and evaluate the accuracy of your model

c. Given the nature of the data, your REST API will likely need to take into account previous transactions, so make sure it is able to take note of transactions from your training dataset as well as previous API calls.

Model
a. We are expecting a machine learning model that can correctly classify whether or not a transaction is fraudulent.

What is the objective of the machine learning model?

We aim to predict the real transactions fraud and the fraud estimated by our model. We will evaluate model performance with the:

F beta score

ROC AUC score

PR AUC score | Average precision
How to work this project.

![Screenshot (15)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/9e66134b-fe93-4af5-bbfd-3fbbdfd9716a)
![Screenshot (14)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/522e9229-572a-4d8f-b6dd-5dea30520ba5)
![Screenshot (13)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/83d3eb4e-c46b-4d54-bcac-878db343a2d8)
![Screenshot (12)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/f6e998e0-a43b-4c85-8ead-
7ffb3613fb13)
![Screenshot (11)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/5d1c1953-994c-40d4-ba4b-565eaeee055d)
![Screenshot (10)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/542f3964-c04d-4370-8766-ac43918ca2b1)
![Screenshot (9)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/8b4515a0-7e91-42ee-8a2d-24b674268f23)
![Screenshot (8)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/8cb07590-17b9-43b6-a20a-f9fb2a396bef)
![Screenshot (7)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/5eea7c5e-ac8f-4a31-82ff-8fc6a16d8804)
![Screenshot (6)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/dbfaa1bd-374f-4949-a703-66c60da4e0cc)
![Screenshot (5)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/3dcbd65a-61eb-4ae9-9c3c-c3433e6b43f0)
![Screenshot (4)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/7875aef3-e668-40f0-9ca0-49191fd918c5)
![Screenshot (3)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/2f3f4ac4-4ddf-46e3-851f-29148c8fcaf8)
![Screenshot (2)](https://github.com/sharma121219/The-Secure-Framework-to-Develop-Income-Tax-Fraud-Detection-using-AI-ML-Techniques/assets/139925541/ee18a241-3050-4564-a7a6-2ce35f80e795)

