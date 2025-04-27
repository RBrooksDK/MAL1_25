<h1 align="center">12 Exam Preparation and Q/A</h1>

Please read the following exam description:

---

## Examination Description
**Course**: Introduction to Machine Learning and AI (MAL1)  
**Examination Format**: Oral Examination  
**Duration**: 20 minutes  

---

**Description**:

The examination is a 20-minute oral examination conducted as a focused discussion. It is based on the six group assignments that the student has submitted during the semester, in accordance with the specified deadlines.

---

**Examination Structure and Procedure**:

At the start of the examination, two assignments from the set of six submitted group assignments will be drawn at random for discussion.

The first assignment drawn will serve as the primary focus for the main, in-depth discussion. The second assignment drawn will be subject to a more brief discussion.

- The first part of the examination will focus on the primary assignment. The student will be expected to briefly demonstrate or describe their solution and engage in a detailed discussion covering the problem, their approach, implementation details (including their code), and results.

- The second part of the examination will involve a shorter discussion of the secondary assignment, focusing on specific concepts or challenges related to that assignment.

---

**Nature of the Examination**:

The examination is explicitly a discussion between the student and the examiner(s). **It is not a presentation**. The student must be prepared to explain, justify, and elaborate on their submitted work and related concepts in response to questions.

---

**Expectations**:

Students are expected to demonstrate thorough understanding of their submitted assignment solutions, including all aspects of their code, the algorithms used, design choices, and results. Students must be prepared to explain every part of their code.

In addition to discussing the specifics of the assignments, students must be prepared to answer questions about theoretical concepts, principles, and algorithms covered throughout the entire course curriculum, as these form the foundation for the assignments.

---

**Note on Code Comments**:

Code should be as clear and self-explanatory as possible **without relying on comments**.  
Only minimal comments are acceptable, such as brief notes on major sections or non-obvious technical decisions.  
**Comments that explain what the code does, describe theory, or restate the logic of the code are not acceptable and will negatively impact the evaluation.**

Students are expected to demonstrate their understanding during the oral discussion, not through excessive code annotation.

---

**Assessment**:

Assessment will be based on the student's demonstration of understanding of their submitted work, their ability to explain technical details and design choices, their grasp of the underlying theoretical principles from the course curriculum, and their active and knowledgeable participation in the discussion.

---

## Expected Knowledge and Discussion Areas

I expect you to be able to explain and discuss:

**Introduction to Machine Learning:**

- what Machine Learning (ML) is, potentially referencing Tom Mitchell's definition ("A computer program learns if its performance improves with experience on a task.")
- the primary reasons for using ML (automating complex tasks, adaptability to changes, handling problems too complex for traditional methods)

- the different types of ML:

     - Supervised Learning (general concept)
     - Unsupervised Learning (general concept)
     - Classification (Supervised, Discrete output)
     - Regression (Supervised, Continuous output)
     - Clustering (Unsupervised, grouping)
     - Dimensionality Reduction (Unsupervised, reducing feature space)
     - the key distinction between Supervised and Unsupervised Learning (labeled vs. unlabeled data)
     - the distinction between Discrete and Continuous variables, particularly in the context of output types for classification and regression

**Challenges in ML:**

- common challenges encountered in ML projects

     - issues related to data quality (insufficient or poor-quality data)
     - issues related to data representativeness (nonrepresentative training data)
     - the concepts of Overfitting (model too complex) and Underfitting (model too simple)

**ML Workflow and Methodologies:**

- the standard steps in an ML workflow (Data Collection, Model Selection, Training, Evaluation, Iteration)

- the importance of gathering a representative training set

- the purpose of the Evaluation step

- how a test set is used to estimate generalisation error

- the purpose of hyperparameter tuning

- how a validation set is used during hyperparameter tuning

- different machine learning methodologies shown:

     - "Train-Test" methodology (how data is split and used)
     - "Validation" methodology (how training, validation, and test sets are used, including the role of validation accuracy for tuning)
     - "Cross Validation" methodology (the concept of splitting data into folds, using multiple train/validation splits, and averaging results for tuning)
     - "Leave-one-out Cross Validation" (understanding it as a special case of cross-validation where each validation set is a single data point)

- the principle that the test set should be isolated and used only for the final evaluation

- the note about training the final model on both training and validation data in the Validation methodology

**Data Preparation:**

- the overall stages of data preparation (Data Exploration, Data Cleaning, Feature Selection, Feature Engineering and Data Transformation)

- specific activities within Data Exploration (studying feature characteristics like type, missing values, outliers; identifying targets; visualizing data; studying correlations; identifying potential transformations)

- specific activities within Data Cleaning (handling outliers - keep/remove/replace; filling missing values and common methods like max/min/0, mode/median/mean, imputation using regression)

- the goal of Feature Selection (dropping irrelevant features)

- different approaches to Feature Selection (correlation analysis, feature selection models, domain knowledge, data quality checks)

- specific techniques in Feature Engineering and Data Transformation (discretizing continuous features, using one-hot encoding, adding transformations like $log(x)$, $sqrt(x)$, $x^2$, aggregating features, scaling, decomposition like date components, dimensionality reduction)

- the ideal timing for performing data cleaning and feature engineering relative to splitting data (ideally only on training and validation data, isolating test data)

- practical considerations and potential compromises in data preparation timing (sometimes done on all data before splitting off test)

**Classification Details:**

- the definition of classification (predicting discrete class labels)

- specific Classification Models mentioned and their core ideas:
     - K-NN (K-Nearest Neighbors): Explain it as an instance-based learner, how it classifies a new data point based on the majority class of its 'k' nearest neighbors, and how distance metrics are crucial for determining 'nearest'.
     - Naive Bayes: Explain it as a probabilistic classifier based on Bayes' theorem and the key "naive" assumption of feature independence.
     - Logistic Regression: Explain it as a linear model used for classification, specifically how it uses the sigmoid function to map a linear combination of features to a probability between 0 and 1.
     - Support Vector Machines (SVM): Explain the core idea of finding the optimal hyperplane that maximizes the margin between different class instances.
     - Tree-based models:
         - Decision Tree: Explain the basic concept of recursively splitting the data based on feature values to create a tree-like structure for classification.
         - Random Forest: Explain it as an ensemble method that builds multiple decision trees and combines their predictions (e.g., through voting) to improve robustness and accuracy. Explain what is "random" in Random Forest (randomly selecting subsets of features and data points for each tree).
         - Gradient Boosted Trees: Explain it as another ensemble method that builds trees sequentially, where each new tree corrects the errors of the previous ones, focusing on misclassified instances.
     - Neural Networks: Reiterate that various types of Neural Networks (like Feedforward, Convolutional, Recurrent) are also used effectively for classification tasks, leveraging layers of interconnected neurons and non-linear activation functions

- why Accuracy alone can be misleading, especially with imbalanced datasets (e.g., the "not 5" example)

- the importance of other performance metrics for classification

- the Confusion Matrix and its components (True Positives (TP), False Positives (FP), True Negatives (TN), False Negatives (FN))

- Precision (definition, TP/(TP+FP), interpretation)

- Recall (definition, TP/(TP+FN), interpretation, synonym Sensitivity)

- F1-Score (definition as the harmonic mean of precision and recall)

- the concept of the Precision-Recall Trade-Off

- how adjusting decision thresholds affects precision and recall

- mention using precision-recall or ROC curves to find a balance

**Regression Details:**

- the definition of Regression (predicting continuous values, objective often minimizing error)

- standard linear regression prediction

- vectorized linear regression prediction

- the typical objective function for regression (Minimize Mean Squared Error (MSE))

- different training methods for regression (Normal Equations, Gradient Descent, Singular Value Decomposition)

- how the Normal Equation computes the optimal parameters directly

- Regularisation Techniques in Regression (purpose: reducing overfitting by penalizing large coefficients)

- the concept of adding a penalty term (lambda * R(beta)) to the loss function (L = MSE + lambda * R(beta))

- the role of the regularisation parameter (lambda or alpha)

- different types of regularization (L2/Ridge, L1/Lasso, Elastic Net)

- the difference between L2 (Ridge) reducing effective dimensionality and L1 (Lasso) reducing actual dimensionality (leading to sparse models)

- Performance Metrics in Regression: MAE, MSE, RMSE (use cases - general interpretability, penalizing errors, comparable units)

- R-squared (R^2): what it represents (variance explained), why it can be negative

- Explained Variance: its relationship to R^2 when predictions are unbiased, why it's always between 0 and 1

**Dimensionality Reduction Details:**

- different approaches to dimensionality reduction (feature selection, model regularization (L1/Lasso), combining/mapping features)

- methods for combining/mapping features (Linear combination/projection, Nonlinear combination)

- Principal Component Analysis (PCA): what it tries to find (global structure), how it works geometrically (finding projection directions that maximize variance), the concept of orthogonal components

- the PCA algorithm (centering data, computing covariance matrix, eigenvalue decomposition, sorting eigenvalues/eigenvectors, projecting data)

- the orthogonal nature of PCA components (orthogonal directions in the original space) and its implications (independence of components)

**Clustering Details:**

- the definition of clustering (grouping similar data points)

- the difference between clustering and classification (no labels in clustering)

- the purpose of clustering (finding structure in data)

- I expect you to be able to explain and discuss:

- k-means clustering:
     - algorithm steps
     
     - challenges (initialisation sensitivity, cluster assumptions)
     
     - improvements (k-means++)

- DBSCAN:
     - algorithm steps
     - core idea of density-based clustering (finding dense regions)
     - concept of density-based clustering
     - parameters $\epsilon$ and min_samples
     - detection of noise points

- hierarchical (agglomerative) clustering:
     - merging based on distance metrics
     - different linkage criteria (single, complete, average, Ward's method)
     - dendrograms (tree-like structure for visualizing clusters)
     - cutting dendrograms to form clusters

**Gradient Descent:**

- the core idea of Gradient Descent for regression (iteratively adjusting parameters to minimize the cost function)

- the steps involved in Gradient Descent (Initialization, Compute Gradient, Update Parameters, Repeat)

- the role of the learning rate (eta) in Gradient Descent (determines step size)

- when Gradient Descent stops (when the cost function converges)

**Neural Network Fundamentals:**

- the basic idea of artificial neurons (inspired by biological neurons)

- the core components of an artificial neuron (inputs, weights, bias, activation function)

- the basic calculation a neuron performs (weighted sum of inputs + bias)

- how artificial neurons form Artificial Neural Networks (ANNs) by being linked in layers

- the general roles of the Input, Hidden, and Output layers

- the purpose of weights (trained during learning)

- the purpose of activation functions (introducing non-linearity)

- common activation functions discussed:

     - Sigmoid (use case: binary classification output, reason)
     - Softmax (use case: multi-class classification output, reason)
     - Linear (use case: regression output, reason)

- Backpropagation: its main purpose (computing gradients of the loss w.r.t weights/biases)

**Code:**

YOU MUST BE ABLE TO EXPLAIN YOUR CODE!

- the structure of your code (functions, classes, modules)
- the purpose of each function and class
- the logic behind your code
- the algorithms you implemented