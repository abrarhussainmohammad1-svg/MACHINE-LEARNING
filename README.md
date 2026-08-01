# MACHINE-LEARNING

### OK, so what exactly is machine learning?  

To define machine learning, first let’s define a more general term: artificial intelligence.

#### **What is artificial intelligence?**

Artificial intelligence (AI) is a general term, which we define as follows:

**artificial intelligence:** The set of all tasks in which a computer can make decisions

# What is machine learning?

Machine learning is similar to artificial intelligence, and often their definitions are confused.

Machine learning (ML) is a part of artificial intelligence, and we define it as follows:

**machine learning:** The set of all tasks in which a computer can make decisions based on
data.

in fig; Machine learning is a part of artificial intelligence.

<img width="414" height="201" alt="image" src="https://github.com/user-attachments/assets/523c440d-cf81-4908-a3d0-0a97c155c9f1" />

Let’s go back to looking at how humans make decisions. In general terms, we make decisions in the following two ways:

   • By using logic and reasoning

   • By using our experience

For example, 

Imagine that we are trying to decide what car to buy. We can look carefully at the features of the car, such as price, fuel consumption, and navigation, and try to figure out the best combination of them that adjusts to our budget. That is using logic and reasoning. If instead we ask all our friends what cars they own, and what they like and dislike about them, we form a list of information and use that list to decide, then we are using experience (in this case, our friends’ experiences).

Machine learning represents the second method:

making decisions using our experience.

In computer lingo, the term for experience is data. Therefore, in machine learning, computers make decisions based on data. Thus, any time we get a computer to solve a problem or make a decision using only data, we are doing machine learning.

We could describe machine learning in the following way:

Machine learning is common sense, except done by a computer.

Going from solving problems using any means necessary to solving problems using only data may feel like a small step for a computer, but it has been a huge step for humanity. Once upon a time, if we wanted to get a computer to perform a task, we had to write a program,
namely, a whole set of instructions for the computer to follow. This process is good for simple tasks, but some tasks are too complicated for this framework.

For example, consider the task of identifying if an image contains an apple. If we start writing a computer program to develop this
task, we quickly find out that it is hard.

In Simple, 

Machine learning encompasses all the tasks in which computers make decisions based on data.
In the same way that humans make decisions based on previous experiences, computers can make decisions
based on previous data.

<img width="444" height="193" alt="image" src="https://github.com/user-attachments/assets/610e0cba-5fe9-4608-82ca-00172d25d3c0" />

### what is deep learning?

In the same way that machine learning is part of artificial intelligence, deep learning is a part of machine learning. One of these techniques has been performing tremendously well, so it has its own field of study called **deep learning (DL)**.
Define as:

**deep learning:** The field of machine learning that uses certain objects called neural networks

Deep learning is a part of machine learning.

<img width="405" height="195" alt="image" src="https://github.com/user-attachments/assets/b1e95cb4-17e6-4928-a7c2-ad2430af8dd8" />

Deep learning is arguably the most used type of machine learning because it works really well. If we are looking at any of the cutting-edge applications, such as image recognition, text generation, playing Go, or self-driving cars, very likely we are looking at deep learning in some way or another.

## How do we get machines to make decisions with data? The remember-formulate-predict framework

In this section, we learn what is meant by making decisions based on data and how some of these techniques work.

For this, let’s again analyze the process humans use to make decisions based on experience. This is what is called **the remember-formulate-predict framework.** The goal of machine learning is to teach computers how to think in the same way, following the same framework.

#### How do humans think?

When we, as humans, need to make a decision based on our experience, we normally use the following framework:
  1. We remember past situations that were similar.
  2. We formulate a general rule.
  3. We use this rule to predict what may happen in the future.

For example, if the question is, “Will it rain today?,” the process to make a guess is the following:

1. We remember that last week it rained most of the time.
2. We formulate that in this place; it rains most of the time.
3. We predict that today it will rain.

We may be right or wrong, but at least we are trying to make the most accurate prediction we can
based on the information we have.

## Models and Algorithms

**Model:** A set of rules that represent our data and can be used to make predictions

**Algorithm:** A procedure, or a set of steps, used to solve a problem or perform a computation. The goal of an algorithm is to build a model.

In short, a model is what we use to make predictions, and an algorithm is what we use to build
the model. Those two definitions are easy to confuse and are often interchanged, but to keep
them clear.

### Some examples of models that humans use

In this section we focus on a common application of machine learning: spam detection.

In the following examples, we will detect spam and non-spam emails. Non-spam emails are also
referred to as **ham**.

**spam and ham:** **_Spam_** is the common term used for junk or unwanted email, such as chain letters, promotions, and so on. The term comes from a 1972 Monty Python sketch in which every item in the menu of a restaurant contained Spam as an ingredient. 

Among software developers, the term **_ham_** is used to refer to non-spam emails.

#### Example: An annoying email friend

In this example, our friend Bob likes to send us email. A lot of his emails are spam, in the form of chain letters. We are starting to get a bit annoyed with him. It is Saturday, and we just got a notification of an email from Bob. Can we guess if this email is spam or ham without looking at it?

To figure this out, we use the remember-formulate-predict method. First, let us remember,
say, the last 10 emails that we got from Bob. That is our data. We remember that six of them were
spam, and the other four were ham.
