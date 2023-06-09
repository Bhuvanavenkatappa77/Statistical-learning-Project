[ece730project.pdf](https://github.com/Bhuvanavenkatappa77/Python-Projects/files/11006653/ece730project.pdf)



Feature selection method:
Compute the variance for each feature, and select the features whose variance is greater than a threshold.

Simulated data:
Suppose that there are K ≥ 2 classes and p features. The first p1 < p features determine the class label and the remaining features are irrelevant. First, select K p1 × 1 vectors mk, k = 1, . . . , K, where all vectors are different, then append p − p1 zeros to each of these vectors to form p × 1 vectors μk, k = 1, . . . , K. Generate nk data points from the Gaussian distribution with mean equal to μk and covariance σ2I, where I is the p × p identify matrix; these are nk data points from the kth class. Generate data points for all K classes to get a training dataset of n = 􏰘Kk=1 nk samples.

Real data:
Two datasets from the book “The Elements of Statistical Learning” by Hasite, Tib- shirani, and Friedman: the spam dataset and the zip code dataset, both are available at https://web.stanford.edu/∼hastie/ElemStatLearn/

1. Implement the classifier with and without feature selection.
2. Use simulated data to investigate the performance of the classifier. More specifically, you need to investigate how the classification error is affected by the noise level (σ2), the number of features p, the number of relevant feature p1, the number of training data samples n, and the feature selection method, ect.
3. Select one real dataset, and run your classifier on the real dataset, compare the per- formance of the classifier with and without feature selection.


[FINAL PROJECT REPORT SL.pdf](https://github.com/Bhuvanavenkatappa77/Python-Projects/files/11006651/FINAL.PROJECT.REPORT.SL.pdf) 




RealDataset2(Case1–withfeatureselection)
• Download the data which includes three iris species with 50 samples each as well as some properties about each flower.
It is one of the classic examples to work on the classifier and its performance Chi2- contingency is considered to select features with maximum correlation
with the final class.

(Case2 – Without Feature selection)
• •
 Consider selecting random features, say, with least correlation. We can even
compare the result by taking the reference.
  Hence passing the data into the classifier.

Results and Discussions- 
This dataset as it is a classic data frame for classification tests, usually used in the competitions. The results, the accuracy score and KNN best score post cross validation everything shows clear difference if the rightful features aren’t selected for the classification. The plots used to depict the classification result also show a huge difference. The classification report doesn’t change because it is associated with the precision and accuracy of the classifier. We can also observe, than the categorical data, the KNN classifier works the best with classical classification dataset, it seems more compatible and as we have observed, it yields more accuracy. In one of the cases, the test accuracy even goes up to 100%,
it indicates, the dataset is clean and compatible with the classifier as well.

SIMULATED DATA IMPLEMENTATION

The data is simulated in the way it is instructed in the project file.
“Suppose that there are K ≥ 2 classes and p features. The first p1 < p features determine the class label, and the remaining features are irrelevant. First, select K p1 × 1 vectors mk, k = 1, . . . , K, where all vectors are different, then append p − p1 zeros to each of these vectors to form p × 1 vectors μk, k = 1, . . . , K. Generate nk data points from the Gaussian distribution with mean equal to μk and covariance σ2I, where I is the p × p identify matrix; these are nk data points from the kth class. Generate data points for all K classes to get a training dataset of n = �Kk=1 nk samples. “
Case1:
• The values of p1, k is show in the image below, considering the values we proceed with applying the KNN classifier.

Case-2
• It’s given in the project detail to change few of the parameters so as to keenly examine the behavior and performance of the classifier.
• “Use simulated data to investigate the performance of the classifier. More specifically, you need to investigate how the classification error is affected
by the noise level (σ2), the number of features p, the number of relevant features p1, the number of training data samples n, and the feature selection method, ect. “
Results and Discussion- 
The random data created seems to be clean even before the classification. The duplicate and correlated feature removal showed null results and the visualization added more proof to it. The Pair plot already gives us an idea prior the classification regarding the nature of the simulated data. The data was very clean and classified majorly into two/three classes which can be evidently seen in the graph. Hence, as expected the model, the classifier came out to be 100% accurate in both the cases. We can conclude in such synthetic data the parameters, number of features considered, size of the dataset will not account for the accuracy. Such datasets can be used only for experimentation on the classifiers and to study their performance or to implement any new functionality. Nevertheless, the feature normalization brings changes in the accuracy rate, that again is as expected. The change in n-neighbor number during cross validation brings in changes with respect to the accuracy. In between both the cases, post cross- validation also there wasn’t any major changes until we change the n-neighbor.

Conclusion:
The varied selection of datasets helped us examine the performance of the classifier, by changing the parameters, say n-neighbors and k, p1 values in simulated data. The visualization of data through different kind of plots helped us understand the nature of the dataset which gave me enough clarity on the steps to undertake prior passing it to the classifier. Checking the accuracy of the classifier is important to understand whether the feature selection method was successful and right features were selected for the classification. I have also used different method to check and eliminate the correlated features for obtaining high accuracy. I have chosen 2 real datasets, one of it required binary classification, another categorical data where dataset was to be divided to different labelled categories. As per observation, the KNN classifier will work the best and yield best results with the categorial data. I have represented another plot diagram to show the clear classification of the dataset. Overall, through this project I got a chance to experiment with different datasets and classifier’s change in performance, in turn affected by many parameters associated with the datasets. KNN behaves differently with different sets of data, if we provide the necessary steps, the output will be more accurate. Cases mentioned above clearly depicts the effects on the accuracy and performance of the classifiers if there will be changes in certain parameters or feature extraction method. Hence, it gave me huge scope of experimenting around the number of samples, feature selection, n-neighbors, etc which led to a clear understanding on the implementation of the KNN classifier.

# Python-Projects
