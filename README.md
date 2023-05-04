Download Link: https://assignmentchef.com/product/solved-cse-802-pattern-recognition-and-analysis-homework4
<br>






<ol>

 <li></li>

 <li>Generate 100 random training points from <em>each </em>of the following two distributions: N(20,5) and N(35,5). Write a program that employs the Parzen window technique with a Gaussian kernel to estimate the density, b<em>p</em>(<em>x</em>), using <em>all </em>200 points. Note that this density conforms to a <em>single </em><strong>bimodal </strong>

  <ul>

   <li>[15 points] Plot the estimated density function for each of the following window widths: <em>h </em>= 0.01,0.1,1,10. [Note: You can estimate the density at discrete values of <em>x </em>in the [0,55] interval with a step-size of 1.]</li>

   <li>[10 points] Repeat the above after generating 500 training points from each of the two distributions, and then 1,000 training points from each of the two distributions.</li>

   <li>[5 points] Discuss how the estimated density changes as a function of the window width and the number of training points.</li>

  </ul></li>

 <li>Consider the dataset available <a href="https://www.cse.msu.edu/~rossarun/courses/sp20/cse802/data/hw04_data.txt">here</a><a href="https://www.cse.msu.edu/~rossarun/courses/sp20/cse802/data/hw04_data.txt">.</a> It consists of two-dimensional patterns, <strong><em>x </em></strong>= [<em>x</em><sub>1</sub>, <em>x</em><sub>2</sub>]<em><sup>t</sup></em>, pertaining to 3 classes (<em>ω</em><sub>1</sub>,<em>ω</em><sub>2</sub>,<em>ω</em><sub>3</sub>). The feature values are indicated in the first two columns while the class labels are specified in the last column. The priors of all 3 classes are the same and a 0-1 loss function is assumed. Partition this dataset into a training set (the first 250 patterns of each class) and a test set (the remaining 250 patterns of each class).</li>

</ol>

<ul>

 <li>[10 points] Let</li>

</ul>

<em>p</em>([<em>x</em><sub>1</sub>, <em>x</em><sub>2</sub>]<em><sup>t</sup>|ω</em><sub>1</sub>) <em>∼          N</em>([0,0]<em><sup>t</sup></em>,4<em>I</em>), <em>p</em>([<em>x</em><sub>1</sub>, <em>x</em><sub>2</sub>]<em><sup>t</sup>|ω</em><sub>2</sub>) <em>∼         N</em>([10,0]<em><sup>t</sup></em>,4<em>I</em>), <em>p</em>([<em>x</em><sub>1</sub>, <em>x</em><sub>2</sub>]<em><sup>t</sup>|ω</em><sub>3</sub>) <em>∼         N</em>([5,5]<em><sup>t</sup></em>,5<em>I</em>),

where <em>I </em>is the 2 <em>× </em>2 identity matrix. What is the error rate on the test set when the Bayesian decision rule is employed for classification? Report the confusion matrix as well.

<ul>

 <li>[15 points] Suppose <em>p</em>([<em>x</em><sub>1</sub>, <em>x</em><sub>2</sub>]<em><sup>t</sup>|ω<sub>i</sub></em>) <em>∼ N</em>(<strong><em>µ</em></strong><em><sub>i</sub></em>,<em>Σ<sub>i</sub></em>), <em>i </em>= 1,2,3, where the <strong><em>µ</em></strong><em><sub>i</sub></em>’s and <em>Σ<sub>i</sub></em>’s are <em>unknown</em>. Use the training set to compute the MLE of the <strong><em>µ<sub>i</sub></em></strong>’s and the <em>Σ<sub>i</sub></em>’s. What is the error rate on the test set when the Bayes decision rule using the <em>estimated parameters </em>is employed for classification? Report the confusion matrix as well.</li>

 <li>[15 points] Suppose the form of the distributions of <em>p</em>([<em>x</em><sub>1</sub>, <em>x</em><sub>2</sub>]<em><sup>t</sup>|ω<sub>i</sub></em>), <em>i </em>= 1,2,3 is unknown. Assume that the training dataset can be used to estimate the density at a point using the Parzen window technique (a spherical Gaussian kernel with <em>h </em>= 1). What is the error rate on the test set when the Bayes decision rule is employed for classification? Report the confusion matrix as well.</li>

 <li>[10 points] Implement the 1-nearest neighbor (1-NN) method for classifying the patterns in the test set. What is the error rate of the 1-NN method on the test set? Report the confusion matrix as well.</li>

</ul>

<ol start="3">

 <li>[20 points] The <a href="https://www.cse.msu.edu/~rossarun/courses/sp20/cse802/data/iris_data.txt">iris (flower) dataset</a> consists of 150 4-dimensional patterns belonging to three classes (setosa=1, versicolor=2, and virginica=3). There are 50 patterns per class. The 4 features correspond to (a) sepal length in cm, (b) sepal width in cm, (c) petal length in cm, and (d) petal width in cm. Note that the class labels are indicated at the end of every pattern.</li>

</ol>

Design a <em>K</em>-NN classifier for this dataset. Choose the first 25 patterns of each class for training the classifier (i.e., these are the prototypes) and the remaining 25 patterns of each class for testing the classifier. [Note: Any ties in the <em>K</em>-NN classification scheme should be broken at random.]

<ul>

 <li>In order to study the effect of <em>K </em>on the performance of the classifier, report the confusion matrix for <em>K</em>=1,5,9,13,17,21.</li>

 <li>Plot the classification accuracy as a function of <em>K</em>. Discuss your observations.</li>

</ul>

<ol start="4">

 <li>[10 points] Based on the notation developed in class, write down the Sequential Backward Selection (SBS) algorithm and the Sequential Floating Backward Selection (SFBS) algorithm.</li>

</ol>