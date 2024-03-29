# Read: Class 16

## Data Science Primer
* Machine learning is not about algorithms but is a comprehensive approach to solving problems.
* **What makes machine learning so special?** 
  - Machine learning is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions.For true machine learning, the computer must be able to learn patterns that it's not explicitly programmed to identify.
* **Key Terminology**
 * **Model** - a set of patterns learned from data.
 * **Algorithm** - a specific ML process used to train a model.
 * **Training data** - the dataset from which the algorithm learns the model.
 * **Test data** - a new dataset for reliably evaluating model performance.
 * **Features** - Variables (columns) in the dataset used to train the model.
 * **Target variable** - A specific variable you're trying to predict.
 * **Observations** - Data points (rows) in the dataset.
* ![image](https://elitedatascience.com/wp-content/uploads/2018/05/What-Goes-Into-a-Successful-Model.jpg) 
* The purpose of exploratory analysis is to "get to know" the dataset. 
* Feature engineering is about creating new input features from your existing ones.In general, you can think of data cleaning as a process of subtraction and feature engineering as a process of addition.
* Linear regression suffers from two major flaws:
 - It's prone to overfit with many input features.
 - It cannot easily express non-linear relationships.

* There are two types of parameters in machine learning algorithms.
1. **Model parameters**
  - Model parameters are learned attributes that define individual models.
 e.g. regression coefficients
 e.g. decision tree split locations.
  - They can be learned directly from the training data.
2. **Hyperparameters**
  - Hyperparameters express "higher-level" structural settings for algorithms.
  e.g. strength of the penalty used in regularized regression
  e.g. the number of trees to include in a random forest
  - They are decided before fitting the model because they can't be learned from the data

## Data Wrangling
* **Data wrangling** is the process of reshaping, aggregating, separating, or otherwise transforming the data from one format to a more useful one.
* One of the most common reasons to wrangle data is when there's "too much" information packed into a single table, especially when dealing with time series data.
* Data Wrangling steps:
  1. Set up your environment.
  2. Import libraries and dataset.
  3. Understand the data.
  4. Filter unwanted observations.
  5. Pivot the dataset.
  6. Shift the pivoted dataset.
  7. Melt the shifted dataset.
  8. Reduce-merge the melted data.
  9. Aggregate with group-by.
