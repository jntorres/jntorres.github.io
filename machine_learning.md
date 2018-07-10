## Machine Learning

Many people hear the buzzwords machine learning, artificial intelligence, big data and think magic. These terms are no more than sophisticated mathematical models that try to help us understand the data we have. Here I will talk about the two categories of machine learning at the end of this page you will find some further resources that discuss the math that supports the approaches we present here. 

### Supervised Machine Learning
Often described as a parametric approach meaning that there is an assumption that sample data comes from a population that follows a probability distribution based on a fixed set of parameters. 

Here are some of the basic steps I take to when I want to use a supervised approach:

0. Have your data in a usable format, ie data has been normalized or scaled (if needed). Do you need a train, validation and test set? 
1. Select a model in which you would like to use for your data (ie, linear regression, SVM, random forest, etc.) Many times researcher will select many models and examine how the different models used impacts results and intrepretabilty. 
2. Based on the model select pay attention to an inital parameters needed, hyperpaterater tuning is likley necessary.
3. Apply model to data, often called training
4. Evaluate model performance, hyperparameter tuning (if needed)
5. Select best performing model based on validation set
6. Use trained model for your held out test set. 



### Unsupervised Machine Learning
The opposite of a parametric approach is a nonparametric approach. 
