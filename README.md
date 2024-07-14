# Demo Video

# [Link To Presentation](https://docs.google.com/presentation/d/1aJo0adn8_QEssoMPy-k_051SvupnHfa7/edit?usp=sharing&ouid=106556702476183896177&rtpof=true&sd=true)

***
## Project Description
### **FRAUD DETECTION SYSTEM**
We wish to tackle the Problem Statement of "Behavioural Analytics for Security in Financial Transactions".

4.7 Trillion Dollars! That is the amount of revenue lost every year due to fraudsters. Astonishingly, 93% of banking-related fraud happens online. This shows the pressing need for an improved Anomaly Detection System. 

We propose a novel behavioral analytics system as a SAAS, exploiting ML algorithms for real-time detection of fraudulent transactions. The Machine Learning model will analyze whether the incoming transaction is fraudulent or legitimate. Upon raising the flag for the fraudulent ones, the system also tracks the criminal's IP address to estimate their location for further action. Being a SAAS enables the system to also send alerts to the clients to be wary of  criminals.

To tackle this problem, we propose a **three-pronged solution**: 
1. **Prevention:** We will create an Android Application with inbuilt Spam and Phishing detection, to protect the user from any harm from the beginning. 
2. **Detection:** The Main Website will connect to a database and a fraud detection model. It will classify whether the transaction is a fraud or not 
3. **Mitigation:** Additionally, the webpage will return the GeoLocation of the IP Address. We will also be storing the details to perform Social Network Analysis on the transaction to identify patterns. 

### Our Innovations
1. **Phishing and Spam Detection** on the Edge
2. **GeoSpatial Analysis:** Utilizing IP-based location distance metrics for geographical analysis. 
3. **Real-time Network Analysis:** Analyzes financial transactions in real-time for enhanced security. 
4. **Crypto-Based Authentication:** Implements a hash-based authentication (Zero-Knowledge Protocol) for secure user login. 
5. **Keystroke Analysis:** Utilizes the user's typing pattern to identify the user.

***
## Technology Stack
1. Frontend Technologies : React, Bootstrap 
2. Backend Technologies : NodeJS, Flask (Python) 
3. Database : MongoDB, Firebase 
4. Machine Learning and Pipelines : Tensorflow, Scikit-Learn, Jenkins 
5. APIs : FastAPI
6. Android App : Kotlin
7. Cloud Messaging : Apache Kafka

***
# UI and App
![Image1](https://github.com/Vishwa-docs/Fraud-Detection-System/blob/main/Resources/Spam%20App.jpg)
![Image2](https://github.com/Vishwa-docs/Fraud-Detection-System/blob/main/Resources/WhatsApp%20Image%202024-02-04%20at%2015.19.31.jpeg)

***
## Data
> Taken from [YouData.ai](YouData.ai)

The data used for training our models was sourced from an open source synthetic dataset on kaggle :

- [Dataset Link](https://www.youdata.ai/datasets/661d160afde5d01e5b326b79)

Our novelty comes with our incorporation of time and distance-based measures to train our model to better detect fraudulent transactions. We compute the distance between the last known location of an account and the current location along with the time interval between the transactions to allow the model to learn the anomalous behavior of certain transactions. This location data is sourced from the public IP information available with the transaction packet.

## Model

The model we chose for our approach is the ever-resilient Random Forest. Through a series of attempts, random forest proved to be better than the others for our carefully curated dataset.

## Deployment

The end deliverable is packaged as a React-Flask web app and a Fast API that allows the users to check if a given transaction is fraudulent. The location data is directly taken from the IP information given. The distance metric is calculated after referring to the last known location and time stamp.
