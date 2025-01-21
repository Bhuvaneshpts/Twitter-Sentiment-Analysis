# Twitter-Sentiment-Analysis

First you Install the Kaggle Library because this dataset is having large number of data's in it.

If you normally upload the dataset it will take upto 1 or 2 days for that you create a API token in the kaggle

!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json/kaggle.json

then download the kaggle.json file in that file path is there just copy and paste over it on code.

kaggle datasets download kazanova/sentiment140

Fetch the datasets locally in the colab.

Next Extract the Zip file to csv format.

Import the dependencies

Next done EDA process on the dataset.

After that using of PorterStemmer library to stem the 
content to lower and then split the content.

Print the stemmed content.

Then create X and Y variables.

X = twitter_data['stemmed_content'].values
Y = twitter_data['target'].values

like this

then print X and Y

Split the dataset into two train and test.

After that converting the textual data to numerical data using TfidfVectorizer().

Create the Logistic Regression model to predict the accuracy score for both training and test data.

In last import pickle library to save the pre-trained model.

import pickle 

using this above Command you import the pickle library.

filename = 'trained_model.sav'
pickle.dump(model, open(filename, 'wb'))

This is the syntax for loading the pre-trained model.

It is used for future predictions of outcomes.

Predict the tweet Positive or Negative by the model.
