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
