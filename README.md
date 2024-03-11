# Research-Practicum-I

Title of the project
Unmasking Falsehood with NLP and Deep Learning in New Classification Using Popular Social Media Network.

The threat Fake News poses on the integrity of information dissemination is on the rise. There is the need to unmask some of this falsehood before it causes more harm to society in general.

Some data science task to be completed in the project includes
Text classification such as multi-class classification.
Sentiment Analysis.
Topic modelingAnomaly detection
Fake new detection
World cloud 

Data would be gotten from some popular social media websites such as facebook, reddit etc and also from some articles.

The data will be 
preprocessed 
Feature extraction
Training of model
Validation of the model
Hyperparameter tuning

Some difficulties I am anticipating are in the area of data collection example includes collection tweets which coils take some time. This could be overcomed using other platforms that are easily accessible.

I plan on completing the project in 6 weeks, this will be in order
Data collection
preprocessed 
Feature extraction
Training of model
Validation of the model
Hyperparameter tuning


A preview of the dataset is shown as follows

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/e192e33f-f25d-4c4d-bd09-6d8b4541eef1)

A first glance at the shape of the dataset used showed that it has 2297 dataset each on each of the label that will be observed. There was a null value that was observe in the dataset but discovered to be in the title feature was is not what we would be looking at today. The null value was filled with blank space.

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/c92d4764-9bb1-4ace-8282-f1aa2a521d75)

THE CLEANING AND PREPROCESSING PROCESS

The dataset has some unwanted feature that were taken out for the smooth running of the model training. This include the id and the title of the news that was release.

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/6026da58-665c-455e-84d5-0a8ef3ffd63b)

The label feature was reassigned numbers for easy training.

EXPLORATORY ANALYSIS 

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/74a37989-a08a-4eed-81c5-d530be483bd4)

The description of the dataset could be seen. We look at the length of the title of the news.

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/1ad09e84-90f4-47cd-b129-1f5375a91937)

This represent the length of the text that will be analyzed. More than 4000 characters sample represent the total sample analyzed.

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/39b4eaac-8c1a-4332-95d4-e6505cca0dbe)

The dataset was reshuffled before analysis to prevent overfitting.

WORDCLOUD BEFORE STREMMING PROCESS

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/5fd9b0f6-f8db-42d4-aea8-8a5a16c2a32b)

WORDCLOUD AFTER STREMMING PROCESS

TFIDFVectorizer was used in the preprocessing steps in converting text data in numerical representation that could be used by machine learning model. the importance of each word is taken note off.

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/67e5c3ac-eb12-4e91-a422-f45954fd3077)

The dataset was splitted into trained and test dataset. The feature will be the text feature which is our dependent variable and our target which will be the dependent variable. 20% will be used for training of the dataset while the rest which is the 20% will be used in testing the validity of the trained model.

5 different models were ran and the outcome were compared to know whichis most effective in the evaluation of the dataset and similar dataset.
There were different metrics used in evaluation of the output of the models. This includes
Confusion Matrix
Classification Report
Accuracy score

The result after running a logistic regreesion on the dataset is as follows
![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/ba0cc0d9-295d-4425-a378-cb7c86f9668d)

The result after running a SVC on the dataset is as follows
![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/1532c7a0-6698-4823-a0c4-eaa83e49b05c)

The result after running a Decision Tree on the dataset is as follows
![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/7d62b56d-5f12-4c4a-a388-59ecd70132fe)

The result after running a Decision Tree on the dataset is as follows
![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/00c38c02-5dd1-4761-9838-9e414b04fb69)

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/87893598-9bf0-455a-a3a7-8b8c77c20b28)

Comparing all the scores and analyzing the metrics in the diagrams above, We could see that accuracy is actually low when precision and recall is put into consideration. That being said, The tree models (Decision Tree and Random Forest) did actually perform lower than the (Logistic Regresion and SVC).

![image](https://github.com/adeyeyealex/Research-Practicum-I/assets/77544400/630ef489-5852-484d-a42b-dd72bb7dd2e6)
A barchart of the four models are also done side by side 

LSTM a neural network was also used in evaluating the dataset. Embedding and pad sequences was utilized to ensure uniformity in analysis. The result actually came out good with much hyper-parameter tuning. I realized that the more hyper-parameter tuning that was done led to reduction in accuracy and an increase in loss.
