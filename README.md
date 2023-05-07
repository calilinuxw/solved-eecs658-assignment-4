Download Link: https://assignmentchef.com/product/solved-eecs658-assignment-4
<br>
Deliverables:

<ol>

 <li>Copy of Rubric4.docx with your name and ID filled out (do not submit a PDF)</li>

 <li>Python source code for CompareFeatureSelectionMethods</li>

 <li>Screen print showing the successful execution of</li>

</ol>

CompareFeatureSelectionMethods. (Copy and paste the output from the Python console screen to a Word document and PDF it).

<ol start="4">

 <li>For Part 2, using the PoV formula and the values from the eigenvalue matrix, show that the program calculated the PoV correctly. (see “Deliverable 4 (PoV) Example” on BlackBoard).</li>

 <li>Answers to the following questions for CompareFeatureSelectionMethods:

  <ol>

   <li>Based on accuracy which dimensionality reduction method, PCA, simulate annealing, or the genetic algorithm worked the best?</li>

   <li>For each of the two other methods, explain why you think it did not perform as well as the best one.</li>

   <li>Did the best dimensionality reduction method produce a better accuracy than using none (i.e. the results of Part 1)? Explain possible reasons why it did or did not.</li>

   <li>Did Part 2 produce the same set of best features as Part 3? Explain possible reasons why it did or did not.</li>

   <li>Did Part 2 produce the same set of best features as Part 4? Explain possible reasons why it did or did not.</li>

   <li>Did Part 3 produce the same set of best features as Part 4? Explain possible reasons why it did or did not.</li>

  </ol></li>

</ol>




Assignment:

<ul>

 <li>In this assignment, you will use 2-fold cross-validation of the iris data set using the Support Vector Machine (SVM) machine learning model.</li>

 <li>This assignment has four parts.</li>

 <li>In each part (except the first one) you will use different dimensionality reduction methods on the iris data set.</li>

 <li>For each of the parts, the Python program should display (with a label showing the Part number):

  <ul>

   <li>Confusion matrix o Accuracy metric</li>

   <li>List of features used to obtain the final confusion matrix and accuracy metric.</li>

  </ul></li>

 <li>Name the program CompareFeatureSelectionMethods</li>

 <li>Part 1:

  <ul>

   <li>Use the original 4 features: sepal-length, sepal-width, petal-length, and petal-width.</li>

  </ul></li>

 <li>Part 2:

  <ul>

   <li>Refer to “PCA Feature Transformation” slides 11-14 and “Python</li>

  </ul></li>

</ul>

Example” slides 24-30 in the 9/30 lecture o Perform PCA on the iris data set as shown in slides 24-30. Do not use the scikit PCA library. You can use the library to check your code.

<ul>

 <li>Use PCA to transform the original 4 features (i.e., sepal-length, sepalwidth, petal-length, petal-width) into 4 new features (z<sub>1</sub>, z<sub>2</sub>, z<sub>3</sub>, and z<sub>4</sub>).</li>

 <li>To determine the transformed features (see slide 14):</li>

</ul>

<ul>

 <li><strong>Z</strong> = <strong>XW<sup>T</sup> </strong></li>

 <li>where</li>

 <li><strong>X</strong> = X_centered matrix of original features (i.e., 4-by-150 array/matrix of original iris dataset features)</li>

 <li><strong>W</strong> = eigenvectors matrix (4-by-4 matrix)</li>

 <li><strong>Z</strong> = transformed X_centered matrix of original features (i.e., 4-by150 array/matrix of transformed iris dataset features, z<sub>1</sub>, z<sub>2</sub>, z<sub>3</sub>, and z<sub>4</sub>) o Display the eigenvalues and eigenvectors matrices. o Select a subset of the transformed features, so that PoV &gt; 0.90.</li>

 <li>Display the PoV</li>

 <li>Use the selected subset of transformed features to calculate the confusion matrix and accuracy metric.</li>

 <li>Part 3:

  <ul>

   <li>Use simulated annealing to select the best set of features from the 4 original features (i.e., sepal-length, sepal-width, petal-length, petal-width) plus the 4 transformed features (z<sub>1</sub>, z<sub>2</sub>, z<sub>3</sub>, and z<sub>4</sub>) from Part 2 (for a total of 8 features).</li>

   <li>Set the iterations = 100</li>

   <li>Perturb with randomly selected 1 or 2 parameters (because 1-5% of 8 is &lt;</li>

  </ul></li>

</ul>

1) o c in Pr[accept] = 1 o Use restart value (x) of 10 o Print out for each iteration:

<ul>

 <li>Subset of features</li>

 <li>Accuracy</li>

 <li>Pr[accept]</li>

 <li>Random Uniform</li>

 <li>Status: Improved, Accepted, Discarded, or Restart</li>

 <li>Part 4:</li>

 <li>Use the genetic algorithm we discussed in class to select the best set of features from the 4 original features plus the 4 transformed features from Part 2 (for a total of 8 features).</li>

 <li>For the initial population use the following sets of features:

  <ul>

   <li>z<sub>1</sub>, sepal-length, sepal-width, petal-length, petal-width</li>

   <li>z<sub>1</sub>, z<sub>2</sub>, sepal-width, petal-length, petal-width</li>

   <li>z<sub>1</sub>, z<sub>2</sub>, z<sub>3</sub>, sepal-width, petal-length</li>

   <li>z<sub>1</sub>, z<sub>2</sub>, z<sub>3</sub>, z<sub>4</sub>, sepal-width</li>

   <li>z<sub>1</sub>, z<sub>2</sub>, z<sub>3</sub>, z<sub>4</sub>, sepal-length o Run the algorithm for 50 generations</li>

  </ul></li>

 <li>At the end of each generation, print out the features and the accuracy for the 5 best sets of features and the generation number.</li>

</ul>




Remember:

<ul>

 <li>Your Programming Assignments are individual-effort.</li>

 <li>You can brainstorm with other students and help them work through problems in their programs, but everyone should have their own unique assignment programs.</li>

</ul>