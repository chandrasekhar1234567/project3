>Building and training ML  models with VERTEX AI
>Build and train the AutoML Model using vertex Ai.
->Google cloud console
1.Create a data set we are using credit card fraud detection data set avaliable on bigquery
2.To create a model we need dataset.once the data is uploaded,we can analyze our data in the rows and columns.
3.From the data set details page,we can select train new model ,define our objective-which is classification -labeling examples as either fraud or not.
4.We want to give name to model and under target column we select a class ,this is an integer indicating whether or not a particular transaction was fraudulent,zero for non fraud,one for fraud.
5.In training options section,we will go to the advance option,since this data is heavily imbalanced,less than 1% of the data contains fraudulent transactions we will choose the AUC PRC OPTION which will maximize precision-recall for the less common class.
6.Last step is compute and pricing,here we enter 1 as the number of compute hours for our budget and leave early stopping enabled.Traning our automl model for one compute hour is typically a good start for understanding relationship between the features and labels.
7.Train for more time  to improve model performance then ready to start taining.
8.We can leave the ui and will get an email when  our training job completes.
9.Model is ready now we can explore evaluation metrics-confusion matrix and feature importance.Confusion matrix -percentage of examples
10.Creating end point in vertex AI.
11.In model page deploy to endpoint.
12.Deploy the endpoint,now we get predictions on our model.UI and api for prediction models.