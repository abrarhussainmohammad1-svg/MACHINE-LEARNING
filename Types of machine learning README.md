Programming computers to mimic the human thinking process is challenging, because computers are engineered to store and process numbers,
not make decisions. 

This is the task that machine learning aims to tackle.

Machine learning is divided into several branches, depending on the type of decision to be made.

**Machine learning has applications in many fields, such as the following:**

• Predicting house prices based on the house’s size, number of rooms, and location

• Predicting today’s stock market prices based on yesterday’s prices and other factors of the market

• Detecting spam and non-spam emails based on the words in the e-mail and the sender

• Recognizing images as faces or animals, based on the pixels in the image

• Processing long text documents and outputting a summary

• Recommending videos or movies to a user (e.g., on YouTube or Netflix)

• Building chatbots that interact with humans and answer questions

• Training self-driving cars to navigate a city by themselves

• Diagnosing patients as sick or healthy

• Segmenting the market into similar groups based on location, acquisitive power, and interests

• Playing games like chess or Go

**The main three families of machine learning models are:**

  • **_supervised learning,_**

  • **_unsupervised learning,_** and

  • **_reinforcement learning._**

### What is the difference between labeled and unlabeled data? What is data?

Data is simply information. Any time we have a table with information, we have data. Normally,
each row in our table is a data point. 
For example,

That we have a dataset of pets. In this case, each row represents a different pet. Each pet in the table is described by certain features of that pet.

#### And what are features?

We defined features as the properties or characteristics of the data. If our data is in 
a table, the features are the columns of the table. In our pet example, the features may be size, name, type, or weight. Features could even be the colors of the pixels in an image of the pet. This is what describes our data. Some features are special, though, and we call them labels.

#### Labels?
This one is a bit less straightforward, because it depends on the context of the problem we are 
trying to solve. Normally, if we are trying to predict a particular feature based on the other ones, that feature is the label. If we are trying to predict the type of pet (e.g., cat or dog) based on information on that pet, then the label is the type of pet (cat/dog). If we are trying to predict if the pet is sick or healthy based on symptoms and other information, then the label is the state of the pet (sick/healthy). If we are trying to predict the age of the pet, then the label is the age (a number).

#### Predictions

We have been using the concept of making predictions freely, but let’s now pin it down. The goal of a predictive machine learning model is to guess the labels in the data. The guess that the model makes is called a prediction.

There are two main types of data: 
**_labeled and unlabeled data_**

#### Labeled and unlabeled data

Labeled data is data that comes with labels. Unlabeled data is data that comes with no labels.

An example of labeled data is a dataset of emails that comes with a column that records whether the 


