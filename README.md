# Notebooks
This is the repo for my projects, both finished and in-progress. Here are the ones you should check out:

# [Word2Vec News Analysis and Regression w/ XGBoost](https://nbviewer.jupyter.org/github/chambliss/Notebooks/blob/master/Word2Vec_News_Analysis.ipynb)

In this project, I:
* Clean text data (news article titles and headlines from [this paper](https://www.researchgate.net/publication/322652391_Multi-Source_Social_Feedback_of_Online_News_Feeds))
* Use Word2Vec to create word embeddings, and visualize word clusters on a t-SNE plot
* Create several illuminating visualizations of popularity and sentiment using Seaborn
* Do the same with titles, by averaging the word vectors in each title
* Use model stacking to engineer new features, with the goal of improving performance for a larger popularity model
* Train a model based on title embedding, topic, time since publishing, and sentiment, in order to predict the article's popularity on Facebook

I am no longer actively working on this project, but future directions would include further feature engineering and perhaps joining external data to improve the accuracy of the popularity model.

# [Cleaning, Analyzing, and Visualizing Survey Data in Python]
(https://nbviewer.jupyter.org/github/chambliss/Notebooks/blob/master/Survey%20Data%20Blog%20Post.ipynb)
At work, I've been analyzing a lot of survey data to produce insights for the teams who need it. I came up with a few tricks specific to producing massive amounts of charts and plots for answering various questions, particularly for working with the data as it is structured when exported from SurveyMonkey. Mostly, it involves some setup with pandas, then writing a few carefully-designed functions to output the desired results. Personally, I've found working on survey data to be quite fun, and I hope this tutorial is helpful to anyone out there who's looking to provide more value to their org while sharpening their Python data manipulation skills at the same time. Disclaimer: there may well be a better way of doing things; I wrote these to get the analysis done quickly, as I work in a fast-paced startup environment!

Also, please note that the notebook uses randomly generated data, not data from my employer.

# [Plots and Charts with Altair](https://nbviewer.jupyter.org/github/chambliss/Notebooks/blob/master/Plots%20and%20Charts%20with%20Altair.ipynb)
This is an exploration of Altair, a new plotting library built on top of Vega/Vega-Lite. It is a -very- nice interface for building modern-looking, interactive visualizations. Altair provides an idiomatic API, adding interactivity and tooltips into charts easily, intelligent interpretation of variables, swift within-call aggregations, no more subplotting headaches (chart concatenation is extremely straightforward), and more!  

Sadly, the interactivity doesn't seem to work on GitHub or nbviewer, so please fork the notebook to your own machine (or visit the [Altair documentation](https://altair-viz.github.io/gallery/index.html)) if you'd like to play around with that.

# [Topic Modeling and K-Means Clustering on arxiv Physics Papers](https://nbviewer.jupyter.org/github/chambliss/Notebooks/blob/master/Classification%20and%20Topic%20Modeling%20Practice.ipynb)

Includes:
* Preprocessing the text data (requires significant preprocessing, incl. regex, due to the raw LaTeX format of the papers)
* Creating a feature matrix, using both NMF (Nonnegative Matrix Factorization) and LDA (Latent Dirichlet Allocation)
* Finding topic groups using the feature matrices
* Clustering the documents themselves w/ K-Means

I may come back to this project and try to remove some more of the LaTeX artifacts now that I've had more experience with regular expressions. (I use regex in the project, but it is only partly effective.)

# [Practicing SQL Queries Using sqlite3 in Python](https://nbviewer.jupyter.org/github/chambliss/Notebooks/blob/master/Practicing%20SQL%20Queries%20using%20sqlite3.ipynb)

Recently, I had a take-home case study for an interview. Because I didn't have access to a database, but I wanted to be certain that my SQL queries were correct, I decided to create my own database using `sqlite3` and write a function to generate data similar to that which I'd be working with on the job. 

Includes:
* Setting up a SQL database using `sqlite3`, creating your first table
* Writing a function to reproducibly generate random data, including dates
* Best practices, explanation of SQL syntax and why the queries work
* Sanity checks for ensuring the queries produced the correct results

# [News EDA](https://nbviewer.jupyter.org/github/chambliss/Notebooks/blob/master/News_Analysis_EDA.ipynb)

This project uses the same dataset as the Word2Vec project. It includes:
* Seaborn visualization of article sentiment by topic
* Defining a function to identify the most positive and negative headline by topic

