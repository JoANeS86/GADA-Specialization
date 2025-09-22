# Google Advanced Data Analytics Specialization

## The Nuts and Bolts of Machine Learning

#### <ins>The different types of Machine Learning</ins>

  - Supervised Machine Learning: Uses labeled datasets to train algorithms to classify or predict outcomes.

<p align="center">
  <img src="https://github.com/user-attachments/assets/16d38638-df43-42e7-94c7-e3157741294d" />
</p>

To summarize, supervised machine learning algorithms use data with answers already in it, and use it to make more answers either by categorizing or by
estimating future data.

  - Unsupervised Machine Learning: Uses algorithms to analyze and cluster unlabeled datasets.

<p align="center">
  <img src="https://github.com/user-attachments/assets/887baef6-1fbf-4507-b275-5414bd84db9f" />
</p>

There are a couple of other types of machine learning besides supervised and unsupervised, like **Reinforcement Learning** or **Deep Learning**.

ML and AI refer to the same principle; training a computer to detect patterns in data without being explicitly
programmed to do so.

Supervised learning models that make predictions that are on a continuum are called **regression algorithms**.

    Continuous variables: Variables that can take on an infinite and uncountable set of values.
    
    Categorical variables: Variables that contain a finite number of groups or categories.
    
    Discrete features: Features with a countable number of values between any two values.

**Discrete variables are able to be counted, and categorical variables are able to be grouped**.

Knowing what type of features you have in a dataset, and what outcomes you're looking for, will help you to determine the most applicable ML model.

<p align="center">
  <img src="https://github.com/user-attachments/assets/dfd94014-2746-4de8-81f3-ff3e9fddf62d" />
</p>

  - Recommendation Systems: Unsupervised learning techniques that use unlabeled data to offer relevant suggestions to users. The main goal of a
Recommendation System is to quantify how similar one thing is to another.

One approach used by Recommendation Systems is Content-based filtering, where comparisons are made based on attributes of content.

Another one is, Collaborative filtering, where comparisons are made based on who else liked the content (the Recommendation System doesn't need to 
know anything about the content itself).

Natural Language Processing, or NLP, could be used too (document-term matrix: A mathematical matrix that describes the frequency of terms that occur 
in each document in a collection.)

Build ethical models

<p align="center">
  <img src="https://github.com/user-attachments/assets/e3b3fe71-1ec5-4270-9207-10da2a798be5" />
</p>

  - Integrated Development Environment (IDE): A piece of software that has an interface to write, run, and test a piece of code.

The two main types of Python files are known as Python scripts and Python notebooks.

    Python scripts are better for production-grade code, and are easier to debug and manage.

    Python notebooks are better for exploratory analyses, presentations, or anything that needs to be human-facing. You are
    able to insert images, text, and links directly into the code.

More about Python packages

<p align="center">
  <img src="https://github.com/user-attachments/assets/3d70a59b-de09-4f30-8129-a8d8a71a63e0" />
</p>

Generally, there are 3 types of Python packages:

  - Operational packages: They load, structure and prepare the dataset for further analysis (E.g., Pandas, Numpy, Scipy).
  - Data Visualization packages: They allow you to create plots and graphics of data (E.g., Matplotlib, Seaborn, Plotly).
  - Machine Learning packages: They give many functions to help build models from a dataset, along with functionality to examine
    the model once it has been built (E.g., Sklearn).

Apart from these, Python has thousands and thousands of packages publicly available.

#### <ins>Workflow for building complex models</ins>

  - Plan

In this section, the course is focused on ML, so it'll continue with an example related to it. But putting that apart, you need to think about whether you need a model in the first place! Many analytical tasks do not
require the creation of a model, and you could spend time creating something that is not necessary to what you’re trying to achieve.

Let's continue with ML and knowing what you need for a problem: The first thing to do when forming your plan is to consider the end goal, and something that can be determined immediately is what type of machine learning
model you’ll need.

    Supervised models are used to make predictions about unseen events. These types of models use labeled data, and the model
    will use these labels and the predictor variables present to learn from the dataset. And when given new data points,
    they’re able to make a prediction of the label.

    Unsupervised models, on the other hand, don’t really make predictions. They are used to discover the natural structure
    of the data, finding relationships within unlabeled data.

  - Analyze

The main focus of the analyze stage is to develop a deeper understanding of the data, while keeping in mind what the model needs to eventually predict.

**Feature engineering** is the process of using practical, statistical, and data science knowledge, to <ins>select, transform, or extract</ins> characteristics, properties, and attributes, from raw data.

    Feature selection: The goal of this type of feature engineering is to select the features in the data that contribute the
    most to predicting your response variable. In other words, you drop features that do not help in making a prediction.
    
    Feature transformation: In feature transformation, data professionals take the raw data in the data set and create features
    that are suitable for modeling. This process is done by modifying the existing features in a way that improves accuracy when
    training the model (Transformation = Change the existing features).

    Feature extraction: Taking multiple features to create a new one that would improve the accuracy of the algorithm
    (Extraction = Create new features from the data).

Datasets used in the workplace can sometimes require multiple rounds of EDA and feature engineering to get everything in a suitable format to train a model.

Class imbalance: When a dataset has a predictor variable that contains more instances of one outcome that another.

There are two general strategies to balance a dataset, and the method that is better to use generally is decided by how much data you have in the first place: Downsampling and Upsampling.

    Downsampling: Downsampling is the process of making the minority class represent a larger share of the whole dataset simply by
    removing observations from the majority class. It is mostly used with datasets that are large. But how large is large
    enough to consider downsampling? Tens of thousands is a good rule of thumb, but ultimately this needs to be validated by
    checking that model performance doesn’t deteriorate as you train with less data. 

    Upsampling: Upsampling is basically the opposite of downsampling, and is done when the dataset doesn’t have a very large number
    of observations in the first place. Instead of removing observations from the majority class, you increase the number of
    observations in the minority class. 

In both cases, upsampling and downsampling, it is important to leave a partition of test data that is unaltered by the sampling adjustment. You do this because you need to understand how well your
model predicts on the actual class distribution observed in the world that your data represents. In the case of the spam detector example, it’s great if your model can score well on resampled data
that is 80% not spam and 20% spam, but you need to know how it will work when deployed in the real world, where spam emails are much less frequent. This is why the test holdout data is not rebalanced.

Class rebalancing should be reserved for situations where other alternatives have been exhausted and you still are not achieving satisfactory model results (class imbalance isn't always
a problem).






















