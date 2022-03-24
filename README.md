# biometric-classification

In this exercise I demonstrate an unsupervised classfifcation technique, K-Means clustering, and a supervised classification technique, K-Nearest Neighbors, on data concerning orthopaedic patients who should be classified into 'normal' or 'abnormal' based on their measurements. The data is available from https://archive.ics.uci.edu/ml/datasets/Vertebral+Column

For the K-Means implementation, values of 2 and 3 for K were used after a slightly inconclusive elbow plot was created to try and find the optimal value of K. This is because our 'abnormal' category actually turned out to be an amalgamation of two different orthopaedic abnormalities. Thus, K-Means in this case was able to detect a hidden cluster within the data. 

For the K-Nearest Neighbors implementation, the data is split into a training sample and a test sample. Then, a for loop runs the algortihm with different values of K in the range of 1 - 40, to find the optimal value for K on this data. The error rate for each value of K is plotted, where we see 17 is the optimal K value in this case. Then we call a function to print the accuracy of classification. 
