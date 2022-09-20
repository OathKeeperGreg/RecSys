This project is a Recommender System for drug prescriptions based on a real world dataset (MIMIC-III Database). It includes 6 different models that we analyze and compare with certain evaluation metrics.

# Algorithms

 - SVD (Singular Value Decomposition)
 - Item-KNN (Item K-Nearest Neighbour)
 - User-KNN (User K-Nearest Neighbour)
 - NMF (Non-negative Matrix Factorization)
 - MLP (Multi-layer Perceptron neural network)
 - GMF (Generalized Matrix Factorization)

# Evaluation Metrics

- Recall
- Precision
- NDCG
- Toxicity score of the drugs


# Post Hoc Re-Ranking

After evaluating all the models above, for the best performing algorithm (SVD) we apply the Post Hoc Re-Ranking to evaluate the results we get once again and compare the two. We find that this method produces safer results for actual use, as can be seen from the Toy Example towards the end of the code.


# Prerequisites

In order to be able to execute algorithms with neural networks, we installed the package Tensorflow 1.15 and tensorflow-estimator 1.15. In more detail, we installed anaconda which provides many ready-made packages and created a virtual environment as follows:

  - Conda create -n py37 python=3.7
  - Conda activate py37
  - Conda install cornac -c cornac-forge
  - Conda install sklearn
  - Conda install tensforflow==1.15
  - Pip install tensorflow-estimator==1.15


When the environment is set, we open Jupyter Notebook from the Anaconda Navigator menu and open the project. Before running it, we need to change the 10th line of code "folder = 'C:\\Users\\Greg\\Python\\RecSys'" to the path that we have the project (and txt.files) in.

The .txt files are necessary to run the code as they contain the data from MIMIC-III database for relationships between drugs-patients and drug-drug interactions.


# Instructions

- Download and install Anaconda from [Anaconda website](https://www.anaconda.com/products/distribution).
- Open Anaconda Navigator and launch CMD.exe prompt.
- Then install the prerequisites mentioned above to create the virtual environment that is required.
- On the top left drop down menu "Applications on" select py37.
- Launch Jypyter Notebook and navigate to the project folder.
- Open the notebook and on the Jupyter menu select Cell -> Run all.
