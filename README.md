# Myopia-Cluster: Predict Myopia

In this project, I apply unsupervised learning by fitting data to a model and using clustering algorithms to place data into groups. 
I first process the raw data myopia.csv to fit the machine learning models. I use several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, I create a visualization to share my findings.

## Steps:
Part 1: Prepare the Data
Part 2: Apply Dimensionality Reduction
Part 3: Perform a Cluster Analysis with K-means
Part 4: Make a Recommendation



### Part 1: Prepare the Data
* Read myopia.csv into a Pandas DataFrame.
* Remove the "MYOPIC" column from the dataset.
* Standardize my dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.



### Part 2: Apply Dimensionality Reduction
* Perform dimensionality reduction with PCA. 
Note: Rather than specify the number of principal components when I instantiate the PCA model, I state the desired explained variance. 
* Further reduce the dataset dimensions with t-SNE and visually inspect the results. To do this, run t-SNE on the principal components, which is the output of the PCA transformation.
* Create a scatter plot of the t-SNE output. 


### Part 3: Perform a Cluster Analysis with K-means
* Create an elbow plot to identify the best number of clusters with following:
1. I use a for loop to determine the inertia for each k between 1 through 10.
2. I determine where the elbow of the plot is, and at which value of k it appears.



### Part 4: Make a Recommendation
Based on my findings, I share a brief recommendation in your Jupyter Notebook. 
