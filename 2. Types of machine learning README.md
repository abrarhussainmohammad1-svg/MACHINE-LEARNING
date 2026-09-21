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

An example of labeled data is a dataset of emails that comes with a column that records whether the emails are spam or ham, or a column that records whether the email is work related.

An example of unlabeled data is a dataset of emails that has no particular column we are interested in predicting.

<img width="576" height="219" alt="image" src="https://github.com/user-attachments/assets/e95faa0d-74ae-4c8d-9603-00a7dcbfe941" />


We see three datasets containing images of pets. The first dataset has a column 
recording the type of pet, and the second dataset has a column specifying the weight of the pet. These two are examples of labeled data. The third dataset consists only of images, with no label, making it unlabeled data.

Labeled and unlabeled data yield two different branches of machine learning called supervised
and unsupervised learning.

### Supervised learning

The branch of machine learning that works with labeled data.
We can find supervised learning in some of the most common applications nowadays, including 
image recognition, various forms of text processing, and recommendation systems. Supervised 
learning is a type of machine learning that uses labeled data.
In short, the goal of a supervised learning model is to predict (guess) the labels.

Example: 

In the above figure, the dataset on the left contains images of dogs and cats, and the labels 
are “dog” and “cat.” For this dataset, the machine learning model would use previous data to predict the label of new data points. This means, if we bring in a new image without a label, the model will guess whether the image is of a dog or a cat, thus predicting the label of the data point 

A supervised learning model predicts the label of a new data point. In this case, the data point corresponds to a dog, and the supervised learning algorithm is trained to predict that this data point does, indeed, correspond to a dog.

The framework we learned for making a decision was **remember-formulate-predict**. This is precisely how supervised learning works. The model first **remembers** the dataset of dogs and cats. Then it **formulates** a model, or a rule, for what it believes constitutes a 
dog and a cat. Finally, when a new image comes in, the model makes a **prediction** about what it thinks the label of the image is, namely, a dog or a cat.

<img width="539" height="254" alt="image" src="https://github.com/user-attachments/assets/90925372-b4cf-42fd-b66d-d6c4dbb7779d" />


Numbers and states are the two types of data that we’ll encounter in supervised learning models. We call the first type **_numerical data_** and the second type **_categorical data_**. 

**numerical data:** is any type of data that uses numbers such as 4, 2.35, or –199. 

Examples of numerical data are prices, sizes, or weights.

**categorical data:** is any type of data that uses categories, or states, such as male/female or cat/dog/bird. For this type of data, we have a finite set of categories to associate to each of the data points.

Two types of supervised learning models:

**regression models:** are the types of models that predict numerical data. The output of a 
regression model is a number, such as the weight of the animal.
**classification models:** are the types of models that predict categorical data. The output of a classification model is a category, or a state, such as the type of animal (cat or dog).

Two examples of supervised learning models: one regression and one classification.

**Model 1: housing prices model (regression):** 

In this model, each data point is a house. The label of each house is its price. Our goal is that when a new house (data point) comes on the market, we would like to predict its label, namely, its price. 

**Model 2: email spam–detection model (classification):**

In this model, each data point is an email. The label of each email is either spam or ham. Our goal is that when a new email (data point) comes into our inbox, we would like to predict its label, namely, whether it is spam or ham.

Notice the difference between models 1 and 2:

• The housing prices model is a model that can return a number from many possibilities, 
such as $100, $250,000, or $3,125,672.33. Thus, it is a regression model.

• The spam detection model, on the other hand, can return only two things: spam or ham. 
Thus, it is a classification model.

#### Regression models predict numbers

Regression models are those in which the label we want to predict is a number. This number is predicted based on the features.

In the housing example, the features can be anything that describes a house, such as the size, the number of rooms, the distance to the closest school, or the crime rate in the neighborhood.

Other places where one can use regression models follow:

• **Stock market:** predicting the price of a certain stock based on other stock prices and 
other market signals

• **Medicine:** predicting the expected life span of a patient or the expected recovery time, based on symptoms and the medical history of the patient

• **Sales:** predicting the expected amount of money a customer will spend, based on the 
client’s demographics and past purchase behavior

• **Video recommendations:** predicting the expected amount of time a user will watch a 
video, based on the user’s demographics and other videos they have watched

The most common method used for regression is linear regression, which uses linear functions (lines or similar objects) to make our predictions based on the features.

#### Classification models predict a state
Classification models are those in which the label we want to predict is a state belonging to a finite set of states. The most common classification models predict a “yes” or a “no,” but many other models use a larger set of states.

In the email spam recognition example, the model predicts the state of the email (namely, spam or ham) from the features of the email. In this case, the features of the email can be the words on it, the number of spelling mistakes, the sender, or anything else that describes the email.

Another common application of classification is image recognition. The most popular image recognition models take as input the pixels in the image, and they output a prediction of what the image depicts. Two of the most famous datasets for image recognition are MNIST and CIFAR-10. MNIST contains approximately 60,000 28-by-28-pixel black-and-white images of handwritten digits which are labelled 0–9. 

Some additional powerful applications of classification models follow:

• **Sentiment analysis:** predicting whether a movie review is positive or negative, 
based on the words in the review

• **Website traffic:** predicting whether a user will click a link or not, based on the user’s demographics and past interaction with the site

• **Social media:** predicting whether a user will befriend or interact with another user, based on their demographics, history, and friends in common

### Unsupervised learning
**The branch of machine learning that works with unlabeled data.**

Unsupervised learning is also a common type of machine learning. It differs from supervised learning in that the data is unlabeled. In other words, the goal of a machine learning model is to extract as much information as possible from a dataset that has no labels, or targets to predict. 

An unsupervised learning algorithm can group the images based on similarity, even 
without knowing what each group represents.

An unsupervised learning algorithm can still extract information from data. For example, it can group similar elements together.

The main branches of unsupervised learning are **clustering, dimensionality reduction, and generative learning.** 

**clustering algorithms:** The algorithms that group data into clusters based on similarity

**dimensionality reduction algorithms:** The algorithms that simplify our data and faithfully describe it with fewer features 

**generative algorithms:** The algorithms that can generate new data points that resemble the existing data

**Let's study these three branches in more detail:-**

### Clustering algorithms 
It split a dataset into similar groups.

Clustering algorithms are those that split the dataset into similar groups.

**Example:-** 

Let’s go back to the two datasets in the section “Supervised learning”—the housing 
dataset and the spam email dataset—but imagine that they have no labels. This means that the housing dataset has no prices, and the email dataset has no information on the emails being spam or ham.

Let’s begin with the housing dataset. What can we do with this dataset? Here is an idea: we could somehow group the houses by similarity. We could group them by location, price, size, or a combination of these factors. This process is called clustering. Clustering is a branch of unsupervised machine learning that consists of the tasks that group the elements in our dataset into clusters where all the data points are similar.

Now let’s look at the **second example**, the dataset of emails. Because the dataset is unlabeled, we don’t know whether each email is spam or ham. However, we can still apply some clustering to our dataset. A clustering algorithm splits our images into a few different groups based on different features of the email. These features could be the words in the message, the sender, the number and size of the attachments, or the types of links inside the email. After clustering the dataset, a human (or a combination of a human and a supervised learning algorithm) could label these clusters by categories such as  **“Personal,” “Social,” and “Promotions.”**

**Example2:-**
Let’s look at the dataset in below table, which contains nine emails that we would 
like to cluster. The features of the dataset are the size of the email and the number of recipients.

<img width="387" height="249" alt="image" src="https://github.com/user-attachments/assets/5df08873-2aa4-4b90-9895-345dce5edfa5" />


we have grouped the emails by their number of recipients. This would result in two clusters: one with emails having two or fewer recipients, and one with emails 
having five or more recipients. We could also try to group them into three groups by size.But you can imagine that as the table gets larger and larger, eyeballing the groups gets harder and harder. 

<img width="575" height="299" alt="image" src="https://github.com/user-attachments/assets/3858f354-fba9-4cb2-95a6-dcdff2ad6716" />


A plot of the email dataset. The horizontal axis corresponds to the size of the email and the vertical axis to the number of recipients. We can see three well-defined clusters in this dataset.

We can see three well-defined clusters, which are highlighted

<img width="567" height="284" alt="image" src="https://github.com/user-attachments/assets/9def82bb-1f91-44aa-ad6d-f81f27ddd414" />


We can cluster the emails into three categories based on size and number of recipients.
This last step is what clustering is all about.  

As for humans, it’s easy to eyeball the three groups once we have the plot. But for a computer, this task is not easy. Furthermore, imagine if our data contained millions of points, with hundreds or thousands of features. With more than three features, it is impossible for humans to see the clusters, because they would be in dimensions that we cannot visualize. Luckily, computers can do this type of clustering for huge datasets 
with multiple rows and columns.

Other applications of clustering are the following:

• **Market segmentation:** dividing customers into groups based on demographics and 
previous purchasing behavior to create different marketing strategies for the groups

• **Genetics:** clustering species into groups based on gene similarity.

• **Medical imaging:** splitting an image into different parts to study different types of tissue

• **Video recommendations:** dividing users into groups based on demographics and 
previous videos watched and using this to recommend to a user the videos that other 
users in their group have watched

##### More on unsupervised learning models

• **K-means clustering:** this algorithm groups points by picking some random centers of 
mass and moving them closer and closer to the points until they are at the right spots.

• **Hierarchical clustering:** this algorithm starts by grouping the closest points together and continuing in this fashion, until we have some well-defined groups.

• **Density-based spatial clustering (DBSCAN):** this algorithm starts grouping points 
together in places with high density, while labeling the isolated points as noise.

• **Gaussian mixture models:** this algorithm does not assign a point to one cluster but 
instead assigns fractions of the point to each of the existing clusters. 

For example, if there are three clusters, A, B, and C, then the algorithm could determine that 60% of a particular point belongs to group A, 25% to group B, and 15% to group C.

### Dimensionality reduction simplifies data without losing too much information

Dimensionality reduction is a useful preprocessing step that we can apply to vastly simplify our data before applying other techniques. 

For example, let’s go back to the housing dataset. 

Imagine that the features are the following:

• Size

• Number of bedrooms

• Number of bathrooms

• Crime rate in the neighborhood

• Distance to the closest school

This dataset has five columns of data. What if we wanted to turn the dataset into a simpler one with fewer columns, without losing a lot of information? Let’s do this by using common sense. Take a closer look at the five features. Can you see any way to simplify them—perhaps to group them into some smaller and more general categories?
After a careful look, we can see that the first three features are similar, because they are all related to the size of the house. Similarly, the fourth and fifth features are similar to each other, because they are related to the quality of the neighborhood. We could condense the first three features into a big “size” feature, and the fourth and fifth into a big “neighborhood quality” feature. How do we condense the size features? We could forget about rooms and bedrooms and consider only the size; we could add the number of bedrooms and bathrooms or maybe take some other combination of the three features. We could also condense the area quality features
in similar ways. 

**Dimensionality reduction algorithms** will find good ways to condense these features, losing as little information as possible and keeping our data as intact as possible while managing to simplify it for easier process and storage.

<img width="568" height="237" alt="image" src="https://github.com/user-attachments/assets/a36934fe-9eb8-4b45-b45a-48f682a8ec05" />

Dimensionality reduction algorithms help us simplify our data. On the left, we have a housing dataset with many features. We can use dimensionality reduction to reduce the number of features in the dataset without losing much information and obtain the dataset on the right.

### Other ways of simplifying our data:
#### Matrix factorization and singular value decomposition

Clustering can be used to simplify our data by reducing the number of rows in our dataset by grouping several rows into one.

<img width="548" height="234" alt="image" src="https://github.com/user-attachments/assets/d1e02764-291f-47ad-9088-7f0adcf08f5c" />

Dimensionality reduction can be used to simplify our data by reducing the number of columns in our dataset.

<img width="375" height="483" alt="image" src="https://github.com/user-attachments/assets/a5bea604-b264-4b09-aa57-9eb9f797a1eb" />

### Generative machine learning
Generative machine learning is one of the most astonishing fields of machine learning. If you have seen ultra-realistic faces, images, or videos created by computers, then you have seen generative machine learning in action.

The field of generative learning consists of models that, given a dataset, can output new data points that look like samples from that original dataset. These algorithms are forced to learn how the data looks to produce similar data points. 

For example:-
If the dataset contains images of faces, then the algorithm will produce realistic-looking faces. Generative algorithms have been able to create tremendously realistic images, paintings, and so on. They have also generated video, music, stories, poetry, and many other wonderful things. The most popular generative algorithm is **generative adversarial networks (GANs)**, developed by **Ian Goodfellow and his coauthors.**
Other useful and popular generative algorithms are **variational autoencoders**, developed by **Kingma and Welling**, and restricted **Boltzmann machines (RBMs)**, developed by **Geoffrey Hinton.**

As you can imagine, generative learning is quite hard. For a human, it is much easier to determine if an image shows a dog than it is to draw a dog. This task is just as hard for computers.

Thus, the algorithms in generative learning are complicated, and lots of data and computing power are needed to make them work well.

## What is reinforcement learning?
Reinforcement learning is a different type of machine learning in which no data is given, and we must get the computer to perform a task. Instead of data, the model receives an environment and an agent who is supposed to navigate in this environment. The agent has a goal or a set of goals.

The environment has rewards and punishments that guide the agent to make the right decisions to reach its goal. 
This all sounds a bit abstract, but let’s look at an example.

Example: Grid world
In figure,
A grid world in which our agent is a robot. The goal of the robot is to find the treasure chest, while avoiding the dragon. The mountain represents a place through which the robot can’t pass.

<img width="596" height="318" alt="image" src="https://github.com/user-attachments/assets/453af061-e14c-4fce-b9e5-6810a9505a1a" />


We see a grid world with a robot at the bottom-left corner. That is our agent. The goal is to get to the treasure chest in the top right of the grid. In the grid, we can also see a mountain, which means we cannot go through that square, because the robot cannot climb mountains. We also see a dragon, which will attack the robot, should the robot dare to land in its square, which means that part of our goal is to not land over there. This is the game. And to give the robot information about how to proceed, we keep track of a score. The score starts at zero. If the robot gets to the treasure chest, then we gain 100 points. If the robot reaches the dragon, we
lose 50 points. And to make sure our robot moves quickly, we can say that for every step the robot makes, we lose 1 point, because the robot loses energy as it walks.

The way to train this algorithm, in very rough terms, follows: 

The robot starts walking around, recording its score and remembering what steps took it there. After some point, it may meet the dragon, losing many points. Therefore, it learns to associate the dragon square, and the squares close to it with low scores. At some point it may also hit the treasure chest, and it learns to start associating that square and the squares close to it to high scores. After playing this game for a long time, the robot will have a good idea of how good each square is, and it can take the path following the squares all the way to the treasure chest. 

In figure 2, a possible path, although this one is not ideal, because it passes too close to the dragon. Can you think of a better one?

<img width="588" height="372" alt="image" src="https://github.com/user-attachments/assets/75849a01-6f19-4cd6-9904-f1327684a2d9" />

Here is a path that the robot could take to find the treasure chest.

Of course, this is a very brief explanation, and there is a lot more to reinforcement learning.

Reinforcement learning has numerous cutting-edge applications, including the following:

• **Games:** recent advances in teaching computers how to win at games, such as Go or chess, use reinforcement learning. Also, agents have been taught to win at Atari games such as Breakout or Super Mario.

• **Robotics:** reinforcement learning is used extensively to help robots carry out tasks such as picking up boxes, cleaning a room, or even dancing!

• **Self-driving cars:** reinforcement learning techniques are used to help the car carry out many tasks such as path planning or behaving in particular environments.
