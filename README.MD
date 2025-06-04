# MSCS_634_Lab_2:Classification Using KNN and RNN Algorithms 
**(KNN vs RNN on Wine Dataset from sklearn)**

## Purpose
The purpose of this lab is to explore the performance of the classication of two most commonly used supervised learning algorithms: **K-Nearest Neighbors (KNN)** and **Radius Neighbors Classifier(RNN)** using the data sets from sklearn.datasets. The main objective is to understand how the two algorithms differ from one another and hows the multiple parameter values (number of neighbors in KNN and radius size for RNN) affect the accuracy of the model. Also, the goal is to determine the most optimal setting for both the algorithms. 

### Key Insights
The dataset from the sklearn consisted of 178 values with 14 attributes (13 chemical properties and 1 target class).
Class 0 has 59 samples
Class 1 has 71 samples
Class 2 has 48 samples.

### K-Nearest Neighbors (KNN)
- The k-values used for the evaluation: `1, 5, 11, 15, 21`
- The greatest accuracy was achieved for the k-value 15 which it reached the peak accuracy of **97.2%**
- All the other k-values recorded the accuracy rate of **94.4%**
- It was observed that larger or smaller k-values caused lower accuracy due to over fitting and underfitting.

### Radius Neighbors Classifier (RNN)
- The radius value used for the RNN algorithm were: `350, 400, 450, 500, 550, 600`.
- All the radius values showed similar accuracy rate of **(38.89%)**, which is extremely low in comparision to KNN.
- The lower accuracy rate shows that RNN couldn't find appropiate number of neighbors with in the specified radius values.

### Visualization:

<img width="863" alt="Image" src="https://github.com/user-attachments/assets/ca7f61a7-bfe9-4d70-8307-0b76942024a7" />
<img width="863" alt="Image" src="https://github.com/user-attachments/assets/0f16c7ae-d726-4633-84e8-e28ff227a00e" />


### Comparision and Analysis: 
The result shows that KNN in average has a higher accuracy rate in comparision to RNN.
KNN Accuracy: The accuracy stayed around 94.44% for the majority k values.
RNN Accuracy: The accuracy stayed fixed at 38.89% due to incorrect radius scaling.

- The KNN algorithm was less affected by the parameter choice 
- The RNN shows the requirement of precise tuning for avoiding the empty neighbor regions. In this case the radius value should be made smaller.

### When to Use each model:
**KNN**
- KNN is best suited for dataset with a constant desinity and balanced classes.

**RNN**
- RNN is suitable for dataset with local variation.



