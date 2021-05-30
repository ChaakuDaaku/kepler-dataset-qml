# Exoplanet Detection using Quantum Data Reupload Method

## Problem Statement
Astronomical data analysis has been a celebrated problem for classical machine learning.Exoplanet detection through astronomical data is known for its peculiar challenges for astronomers. Advances in telescope technology have made it possible to install telescopes in space to obtain images from objects lightyears away. However this has given rise to humongous datasets which are difficult to analyse and interpret.
 
Kepler telescope was commissioned in 2009 for detection of exoplanets. Over the years the dataset obtained from the Kepler telescope has gained a reputation in astronomical data analysis similar to MNIST dataset in statistical data analysis. 
 
In recent times, state-of-the-art machine learning approaches including k-nearest neighbour, Principal Component Analysis, Convolution Neural Network, Recurrent Neural Network have been applied to the Kepler's noisy dataset. The results have been encouraging. However they suffer from lack of faster execution and complicated algorithms.The analysis of Kepler astronomical data is  prone to high number of false positives. 
 
Quantum Computing is the latest addition in the line of emerging technologies proving to be a viable solution for the complex problems which take years for classical supercomputer to solve. 
 
Since nearly all latest exoplanet discoveries are made using data science coupled with new approaches. In the year 2020 alone, 261 exoplanets were detected. 
 
Given the specific nature of the Kepler dataset, it is evident to employ techniques of Quantum Computing to take advantage of its inherent parallelism. Quantum entanglement and superposition could prove beneficial to analyse Kepler dataset in faster duration avoiding spurious detection

------
 

## Solution Statement

We have approached the problem of exoplanet detection from the Kepler dataset from a Quantum Computing perspective specifically considering the limit on uses of qubits and faithful representation of data fed into the Quantum Circuit.
 
The Kepler dataset has 9564 rows and 50 columns consisting of observations of sensors as well as a few derived parameters. The dataset is subjected to null values. The labels were in three categories Confirmed, Candidate and False positive. 
 
During pre-processing of the data, labels were converted to binary [0,1] and null values were removed. Out of 49 features of the datasets, most relevant 4 (and 6) features were selected.
 
Data reuploading concept uses a single qubit to represent arbitrarily high dimensional data. Multi-layers learning model strategy allows us to train the Quantum classifier circuit avoiding the problem of barren plateaus and achieve lesser depth circuits successfully. 

In the processing of training the model we used Variational Quantum Circuit for Data reuploading in a five layered quantum network. Each layer has been trained separately using the dataset. Mean-squared-error has been used as the cost function for training the network. 

We performed the simulation of the proposed Quantum network using (i) 4 features and to test the efficiency of the network (ii) 6 features. It was found the 4 features were giving better accuracy and loss values than the network using 6 features. The overall speed of the Quantum network was much faster than its classical counterparts