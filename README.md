# Notebooks
This is the repo for my projects, both finished and in-progress. Here are the ones you should check out:

# [Word2Vec News Analysis and Regression w/ XGBoost](https://github.com/chambliss/Notebooks/blob/master/Word2Vec_News_Analysis.ipynb)

In this project, I:
* Clean text data (news article titles and headlines from this paper)
* Use Word2Vec to create word embeddings, and visualize word clusters on a t-SNE plot
* Create several illuminating visualizations of popularity and sentiment using Seaborn
* Do the same with titles, by averaging the word vectors in each title
* Train a model based on title embedding, topic, time since publishing, and sentiment, in order to predict the article's popularity on each platform

It is currently a work-in-progress, where I am currently exploring the use of model stacking to improve XGBoost's performance.

# [News EDA](https://github.com/chambliss/Notebooks/blob/master/News_Analysis_EDA.ipynb)

This project uses the same dataset. It includes:
* Seaborn visualization of article sentiment by topic
* Defining a function to identify the most positive and negative headline by topic

It is also a work-in-progress.

# [Topic Modeling and K-Means Clustering on arxiv Physics Papers](https://github.com/chambliss/Notebooks/blob/master/Classification%20and%20Topic%20Modeling%20Practice.ipynb)

Includes:
* Reading in tens of thousands of papers and preprocessing the text data (requires significant preprocessing, incl. regex, due to the raw LaTeX format of the papers)
* Creating a feature matrix, using both NMF (Nonnegative Matrix Factorization) and LDA (Latent Dirichlet Allocation)
* Finding topic groups using the feature matrices
* Clustering the documents themselves w/ K-Means

# [Practicing SQL Queries Using sqlite3 in Python](https://github.com/chambliss/Notebooks/blob/master/Practicing%20SQL%20Queries%20using%20sqlite3.ipynb)

Recently, I had a take-home case study for an interview. Because I didn't have access to a database, but I wanted to be certain that my SQL queries were correct, I decided to create my own database using `sqlite3` and write a function to generate data similar to that which I'd be working with on the job. 

Includes:
* Setting up a SQL database using `sqlite3`, creating your first table
* Writing a function to reproducibly generate random data, including dates
* Best practices, explanation of SQL syntax and why the queries work
* Sanity checks for ensuring the queries produced the correct results

