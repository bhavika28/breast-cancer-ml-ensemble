# Breast-Mass-Classification-Using-Decision-Trees-Random-Forests-AdaBoost-and-Naive-Bayes-with-PCA


### Project Title:
**"Breast Mass Classification Using Decision Trees, Random Forests, AdaBoost, and Naive Bayes with PCA for Feature Reduction"**

### Steps for the Project:

#### Step 1: Import the Dataset
- Load the provided dataset of breast mass images with 569 data instances and 30 features from a .csv file.
- The features represent characteristics of cell nuclei extracted from digitized fine needle aspirate (FNA) images.
- Each instance is classified as malignant (1) or benign (0).

#### Step 2: Preprocess the Data
- Handle missing data (if any) and normalize the features for better model performance.
- Split the data into 70% training and 30% testing.

#### Step 3: Decision Tree Classifier
1. **Train a Decision Tree Classifier (DT)**:
   - Train one model using the **Entropy** criterion (C1) and another using **GINI** criterion (C2).
   - Compare their performance by evaluating accuracy on the test set.
   
2. **Visualize the Decision Trees**:
   - Use the `graphviz` library to visualize the trained C1 and C2 models.

3. **Prune the Trees**:
   - Limit the depth of C1 and C2 decision trees to prevent overfitting.
   - Compare the pruned models with the unpruned ones.

4. **Depth Experiment**:
   - Vary the depth of C1 and C2 from 1 to 20 and plot the test set performance for each.
   
5. **Visualize the Best Models**:
   - Choose the best-performing tree depth and visualize both C1 and C2.

#### Step 4: Random Forest Classifier
1. **Train a Random Forest Classifier (RF)**:
   - Start with 10 estimators and compare performance with the decision tree (C1).

2. **Estimator Experiment**:
   - Change the number of estimators to 10, 50, 100, 500, and 1000.
   - Plot the performance (accuracy) on the test set for each.

3. **Cross-Validation**:
   - Perform 5-fold cross-validation on the RF classifier with 50 estimators and report the performance.

4. **Feature Importance**:
   - Train RF with 200 estimators and visualize feature importance using two methods:
     1. **Mean Decrease in Impurity**.
     2. **Feature Permutation**.
   - Explain the differences between the plots.

#### Step 5: AdaBoost Classifier
1. **Train an AdaBoost Classifier**:
   - Train the classifier with 10 estimators and compare the performance with C1 and RF (from Step 4).

2. **Estimator Experiment**:
   - Change the number of estimators to 10, 50, 100, 500, and 1000.
   - Plot the performance (accuracy) on the test set for each.

3. **Cross-Validation**:
   - Perform 5-fold cross-validation on AdaBoost with 50 estimators and report the results.

#### Step 6: Naive Bayes Classifier
1. **Train a Gaussian Naive Bayes Classifier**:
   - Train the model and compare its performance with C1, RF (from Step 4), and AdaBoost (from Step 5).

#### Step 7: Principal Component Analysis (PCA)
1. **Perform PCA**:
   - Use PCA to reduce the dimensionality of the dataset.
   - Print the **Cumulative Proportion** and keep only the features accounting for more than 95% of the total variance.

2. **Compare Reduced Features**:
   - Train an RF classifier with 100 estimators using the reduced feature set and compare the performance to the RF model trained with all features.

---

This structure will help you manage the steps efficiently and report the required outputs like accuracy, visualizations, and cross-validation results. Let me know if you need further details!
