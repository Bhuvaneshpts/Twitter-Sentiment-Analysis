# Twitter-Sentiment-Analysis

Step 1: First you Install the Kaggle Library because this dataset is having large number of data's in it.

If you normally upload the dataset it will take upto 1 or 2 days for that you create a API token in the kaggle

!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json/kaggle.json

then download the kaggle.json file in that file path is there just copy and paste over it on code.

kaggle datasets download kazanova/sentiment140

Step 2: Fetch the datasets locally in the colab.

Step 3: Next Extract the Zip file to csv format.

Import the dependencies

Step 4: Next done EDA process on the dataset.

Step 5: After that using of PorterStemmer library to stem the 
content to lower and then split the content.

Step 6: Print the stemmed content.

Step 7: Then create X and Y variables.

X = twitter_data['stemmed_content'].values
Y = twitter_data['target'].values

like this

then print X and Y

Step 8: Split the dataset into two train and test.

Step 9: After that converting the textual data to numerical data using TfidfVectorizer().

Step 10: Create the Logistic Regression model to predict the accuracy score for both training and test data.

Step 11: In last import pickle library to save the pre-trained model.

import pickle 

using this above Command you import the pickle library.

filename = 'trained_model.sav'
pickle.dump(model, open(filename, 'wb'))

This is the syntax for loading the pre-trained model.

It is used for future predictions of outcomes.

Step 12: Predict the tweet Positive or Negative by the model.

**Technologies used**

Python

Numpy

Pandas

Matplotlib

Seaborn

JupyterNotebook

PorterStemmer

Pickle
