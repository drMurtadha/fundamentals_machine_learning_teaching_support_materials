# Fundamentals of Machine Learning: Teaching Support Materials

## 1. Recommended Course Structure

**Course level:** Undergraduate upper-year or early postgraduate introductory course  
**Duration:** 14 teaching weeks, one semester  
**Weekly contact hours:** 2-hour lecture + 2-hour practical/lab  
**Prerequisites:** Basic programming, introductory statistics, basic linear algebra recommended but not assumed deeply  
**Primary software:** Python, Jupyter Notebook, NumPy, pandas, matplotlib/seaborn, scikit-learn  

### Course Aims

This course introduces the core ideas, algorithms, workflows, and practical tools used in machine learning. Students learn how to frame prediction and pattern-discovery problems, prepare data, train models, evaluate performance, and communicate results responsibly.

### Learning Outcomes

By the end of the course, students should be able to:

1. Explain key machine learning concepts, including supervised learning, unsupervised learning, generalization, overfitting, and model evaluation.
2. Apply regression, classification, tree-based, support vector machine, clustering, and introductory neural network models.
3. Use Python and scikit-learn to build reproducible machine learning pipelines.
4. Evaluate models using appropriate metrics and validation methods.
5. Perform basic feature engineering, preprocessing, and model selection.
6. Interpret model results and communicate limitations clearly.
7. Complete a small end-to-end machine learning project using real or realistic data.

### Suggested Semester Flow

| Phase | Weeks | Focus |
|---|---:|---|
| Foundations | 1-3 | ML concepts, Python workflow, data preparation, supervised vs unsupervised learning |
| Core supervised learning | 4-8 | Regression, classification, model evaluation, trees, random forests, SVMs |
| Unsupervised learning and features | 9-10 | Clustering, dimensionality reduction, feature engineering, pipelines |
| Neural and deep learning basics | 11-12 | Neural networks, backpropagation intuition, deep learning concepts |
| Integration and project work | 13-14 | End-to-end ML workflow, ethics, presentations, revision |

## 2. Weekly Teaching Plan

| Week | Topic | Key Concepts | Suggested Lecture Slide Titles | Practical/Lab Activity |
|---:|---|---|---|---|
| 1 | Introduction to Machine Learning | What ML is; examples; data, features, labels; prediction vs explanation; ML workflow; responsible use | "What Is Machine Learning?"; "Why Machines Learn from Data"; "The ML Workflow"; "Types of ML Problems"; "Risks and Responsible Use" | Set up Python/Jupyter environment. Explore a simple dataset with pandas. Identify features, labels, missing values, and possible prediction tasks. |
| 2 | Python for ML and Data Preparation | NumPy arrays; pandas DataFrames; visualization; train/test split; data leakage; reproducibility | "Python ML Toolkit"; "From Raw Data to Dataset"; "Train/Test Splits"; "Data Leakage"; "Reproducible Notebooks" | Load a CSV dataset, clean missing values, visualize distributions, split data using scikit-learn. |
| 3 | Supervised and Unsupervised Learning | Labels vs no labels; regression vs classification; clustering; generalization; baseline models | "Learning With and Without Labels"; "Regression, Classification, Clustering"; "Generalization"; "Baselines Matter"; "When Not to Use ML" | Compare a baseline classifier/regressor with a simple scikit-learn model. Discuss when unsupervised learning may be useful. |
| 4 | Regression | Simple and multiple linear regression; loss functions; mean squared error; coefficients; underfitting/overfitting | "Predicting Continuous Values"; "Linear Regression Intuition"; "Loss and Error"; "Interpreting Coefficients"; "Overfitting in Regression" | Build linear regression and polynomial regression models. Evaluate with MAE, MSE, RMSE, and R-squared. |
| 5 | Classification | Binary and multiclass classification; logistic regression; decision boundary; confusion matrix; class imbalance | "Predicting Categories"; "Logistic Regression"; "Decision Boundaries"; "Confusion Matrix"; "Imbalanced Data" | Train logistic regression and k-nearest neighbors classifiers. Compare accuracy, precision, recall, F1-score, and ROC-AUC. |
| 6 | Model Evaluation | Train/validation/test; cross-validation; bias-variance trade-off; hyperparameter tuning; evaluation pitfalls | "How Good Is the Model?"; "Validation Strategy"; "Cross-Validation"; "Bias and Variance"; "Evaluation Mistakes" | Use cross-validation and GridSearchCV/RandomizedSearchCV to tune a classifier. Interpret validation vs test results. |
| 7 | Decision Trees | Tree structure; splitting criteria; entropy/Gini; depth; pruning; interpretability | "Learning Rules from Data"; "How Trees Split"; "Tree Depth and Overfitting"; "Interpreting a Tree"; "Strengths and Weaknesses" | Train and visualize a decision tree. Experiment with max_depth and min_samples_leaf. Explain learned rules. |
| 8 | Random Forests and Ensemble Learning | Bagging; random forests; feature importance; variance reduction; comparison with single trees | "Why Ensembles Work"; "Bagging"; "Random Forests"; "Feature Importance"; "Trees vs Forests" | Compare decision tree and random forest performance on the same dataset. Examine feature importance and confusion matrix. |
| 9 | Support Vector Machines | Margin; support vectors; kernels; scaling; linear vs nonlinear classification; SVM hyperparameters | "Maximum Margin Classifiers"; "Support Vectors"; "Kernel Trick Intuition"; "Scaling Matters"; "Tuning C and Gamma" | Train linear and RBF-kernel SVMs on a scaled dataset. Visualize decision boundaries on 2D data. |
| 10 | Clustering and Unsupervised Learning | K-means; hierarchical clustering; DBSCAN; silhouette score; PCA for visualization; interpreting clusters | "Finding Structure Without Labels"; "K-Means"; "Density-Based Clustering"; "Evaluating Clusters"; "PCA for Visualization" | Apply k-means and DBSCAN. Use silhouette score and PCA plots to analyze clusters. |
| 11 | Feature Engineering and Pipelines | Encoding categorical variables; scaling; imputation; feature selection; dimensionality reduction; pipelines | "Features Shape the Model"; "Numerical and Categorical Features"; "Scaling and Imputation"; "Feature Selection"; "scikit-learn Pipelines" | Build a ColumnTransformer and Pipeline for mixed numerical/categorical data. Compare performance before and after preprocessing. |
| 12 | Neural Networks | Perceptron; multilayer perceptron; activation functions; loss; gradient descent; backpropagation intuition | "From Linear Models to Neurons"; "Hidden Layers"; "Activation Functions"; "Learning by Gradient Descent"; "Neural Network Limits" | Train scikit-learn MLPClassifier/MLPRegressor. Compare with logistic regression or random forest. Observe effects of hidden layers and learning rate. |
| 13 | Basic Deep Learning Concepts | Deep networks; representation learning; CNN/RNN/Transformer overview; epochs/batches; regularization; GPUs; ethical concerns | "What Makes Learning Deep?"; "Representations"; "Training Deep Networks"; "Overfitting and Regularization"; "Modern Deep Learning Overview" | Optional Keras/PyTorch demo or guided notebook: train a small image or tabular neural network. Discuss when deep learning is unnecessary. |
| 14 | End-to-End ML Project and Review | Problem framing; data pipeline; model comparison; reporting; limitations; final presentations; course review | "From Dataset to Decision"; "Model Comparison"; "Communicating Results"; "Limitations and Ethics"; "Course Review" | Mini-project presentations or final lab clinic. Students present problem, data, model, evaluation, and limitations. |

## 3. Suitable Textbooks and Open-Access References

### Core Recommended Textbooks

1. Gareth James, Daniela Witten, Trevor Hastie, Robert Tibshirani, and Jonathan Taylor, *An Introduction to Statistical Learning with Applications in Python*. Recommended as the primary conceptual and practical textbook. The official site provides downloadable PDFs and notes that the Python edition was published in 2023.
2. Aurelien Geron, *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow*, 3rd ed. Good for applied Python work, scikit-learn workflows, and accessible deep learning practice.
3. Christopher M. Bishop, *Pattern Recognition and Machine Learning*. Useful as an advanced optional reference for mathematically stronger students.

### Open-Access and Free References

1. *An Introduction to Statistical Learning* official site: free PDFs, labs, and supporting resources.
2. scikit-learn User Guide: official documentation for supervised learning, unsupervised learning, model evaluation, preprocessing, pipelines, and common pitfalls.
3. Google Machine Learning Crash Course: short practical modules on regression, classification, data, neural networks, production ML, and fairness.
4. Marc Peter Deisenroth, A. Aldo Faisal, and Cheng Soon Ong, *Mathematics for Machine Learning*: free PDF for mathematical foundations.
5. Aston Zhang, Zachary C. Lipton, Mu Li, and Alexander J. Smola, *Dive into Deep Learning*: open-source deep learning reference with code-based explanations.
6. The Elements of Statistical Learning: advanced free reference for theory, suitable for instructor preparation or extension readings.

### Suggested Reading Mapping

| Course Topic | Recommended Reading |
|---|---|
| ML overview and workflow | ISL Ch. 1-2; Google ML Crash Course introduction |
| Regression | ISL regression chapters; Google linear regression module |
| Classification | ISL classification chapters; Google logistic regression/classification modules |
| Model evaluation | scikit-learn model selection and evaluation guide |
| Trees and random forests | ISL tree-based methods; scikit-learn tree and ensemble documentation |
| SVM | ISL SVM chapter; scikit-learn SVM guide; MML SVM chapter |
| Clustering | ISL unsupervised learning; scikit-learn clustering guide |
| Feature engineering | scikit-learn preprocessing, feature extraction, pipelines, and common pitfalls |
| Neural networks/deep learning | ISL deep learning chapter; D2L selected introductory chapters |

## 4. Suggested Lecture Slide Titles by Week

### Week 1: Introduction to Machine Learning

- What Is Machine Learning?
- Why Use Machine Learning?
- Data, Features, Labels, and Models
- Supervised, Unsupervised, and Reinforcement Learning
- The End-to-End ML Workflow
- Common ML Applications
- Risks: Bias, Misuse, and Overclaiming

### Week 2: Python for Machine Learning

- The Python ML Environment
- Working with NumPy and pandas
- Exploratory Data Analysis
- Visualizing Data Patterns
- Train/Test Splits
- Reproducibility in Notebooks
- Data Leakage

### Week 3: Supervised and Unsupervised Learning

- Learning from Labeled Data
- Learning from Unlabeled Data
- Regression vs Classification
- Clustering and Pattern Discovery
- Baseline Models
- Generalization
- Choosing the Right Learning Approach

### Week 4: Regression

- Continuous Prediction Problems
- Linear Regression Intuition
- Loss Functions and Least Squares
- Multiple Regression
- Polynomial Features
- Regression Evaluation Metrics
- Underfitting and Overfitting

### Week 5: Classification

- Classification Problems
- Logistic Regression
- Decision Boundaries
- Binary and Multiclass Classification
- Confusion Matrix
- Precision, Recall, F1-Score
- Class Imbalance

### Week 6: Model Evaluation

- Why Evaluation Matters
- Training, Validation, and Testing
- Cross-Validation
- Bias-Variance Trade-Off
- Hyperparameter Tuning
- ROC-AUC and PR Curves
- Evaluation Pitfalls

### Week 7: Decision Trees

- Rule-Based Learning
- Tree Splits
- Gini, Entropy, and Information Gain
- Tree Depth and Complexity
- Pruning and Regularization
- Interpreting Tree Models
- When Trees Fail

### Week 8: Random Forests

- Ensemble Learning
- Bagging
- Random Forest Algorithm
- Feature Importance
- Reducing Variance
- Comparing Trees and Forests
- Practical Tuning

### Week 9: Support Vector Machines

- Maximum Margin Intuition
- Support Vectors
- Linear SVM
- Nonlinear SVM and Kernels
- Feature Scaling
- C and Gamma
- Practical Strengths and Limitations

### Week 10: Clustering

- Unsupervised Learning Goals
- K-Means Clustering
- Choosing K
- Hierarchical Clustering
- DBSCAN
- Silhouette Score
- Visualizing Clusters with PCA

### Week 11: Feature Engineering

- Why Features Matter
- Handling Missing Data
- Scaling Numerical Features
- Encoding Categorical Features
- Feature Selection
- Dimensionality Reduction
- Building Pipelines

### Week 12: Neural Networks

- Perceptrons
- Multilayer Networks
- Activation Functions
- Loss and Optimization
- Backpropagation Intuition
- Regularization
- Neural Networks in scikit-learn

### Week 13: Basic Deep Learning Concepts

- What Is Deep Learning?
- Representation Learning
- CNNs, RNNs, and Transformers at a Glance
- Epochs, Batches, and Learning Rates
- Overfitting in Deep Learning
- GPUs and Frameworks
- Responsible Deep Learning

### Week 14: End-to-End ML Project and Review

- Framing an ML Problem
- Data Preparation Review
- Model Comparison
- Interpreting Results
- Communicating Limitations
- Project Presentations
- Final Exam Review

## 5. Suggested Practical/Lab Activities Using Python

| Lab | Activity | Main Tools | Output |
|---:|---|---|---|
| 1 | Python/Jupyter setup and dataset exploration | Jupyter, pandas, matplotlib | Short exploratory notebook |
| 2 | Data cleaning and train/test split | pandas, scikit-learn | Cleaned dataset and split strategy |
| 3 | Baseline models | DummyClassifier, DummyRegressor | Baseline performance report |
| 4 | Linear and polynomial regression | LinearRegression, PolynomialFeatures | Regression comparison notebook |
| 5 | Classification with logistic regression and k-NN | LogisticRegression, KNeighborsClassifier | Classification metrics table |
| 6 | Cross-validation and hyperparameter tuning | cross_val_score, GridSearchCV | Validation report |
| 7 | Decision tree visualization | DecisionTreeClassifier, plot_tree | Interpreted tree diagram |
| 8 | Random forest model comparison | RandomForestClassifier/Regressor | Feature importance analysis |
| 9 | SVM with scaling and kernels | StandardScaler, SVC | Decision boundary visualization |
| 10 | Clustering and PCA visualization | KMeans, DBSCAN, PCA | Cluster interpretation report |
| 11 | Feature engineering pipeline | ColumnTransformer, Pipeline, OneHotEncoder | End-to-end preprocessing pipeline |
| 12 | Neural network experiment | MLPClassifier/Regressor | Model tuning log |
| 13 | Optional deep learning demo | Keras or PyTorch | Guided neural network notebook |
| 14 | Project clinic/presentation | Full Python stack | Final project notebook and presentation |

### Recommended Datasets

- scikit-learn built-in datasets: Iris, Breast Cancer, Wine, Diabetes, California Housing
- OpenML datasets accessible through scikit-learn
- UCI Machine Learning Repository datasets
- Kaggle classroom-safe datasets, where licensing permits
- Locally relevant datasets from public government/open data portals

## 6. Suggested Assignments, Mini-Projects, and Assessment Components

### Assessment Structure

| Component | Weight | Description |
|---|---:|---|
| Lab participation and short lab submissions | 15% | Weekly practical tasks submitted as notebooks or short reports |
| Assignment 1: Data preparation and regression | 15% | Clean a dataset, perform EDA, build regression models, evaluate results |
| Assignment 2: Classification and model evaluation | 20% | Build multiple classifiers, tune hyperparameters, compare metrics, discuss limitations |
| Mini-project | 25% | End-to-end ML project using a dataset selected or approved by instructor |
| Final test/exam | 25% | Conceptual understanding, interpretation, evaluation, and short applied questions |

Alternative for more project-based delivery:

| Component | Weight |
|---|---:|
| Weekly labs | 20% |
| Two technical assignments | 30% |
| Group mini-project | 35% |
| Individual reflection/viva | 15% |

### Assignment 1: Regression and Data Preparation

**Objective:** Build and evaluate regression models on a tabular dataset.

**Required tasks:**

- Define the prediction problem.
- Conduct exploratory data analysis.
- Handle missing values and outliers where appropriate.
- Split data into training and test sets.
- Train at least two regression models.
- Evaluate using MAE, RMSE, and R-squared.
- Discuss underfitting, overfitting, and limitations.

### Assignment 2: Classification and Evaluation

**Objective:** Compare classification models using suitable metrics.

**Required tasks:**

- Train at least three classifiers, such as logistic regression, decision tree, random forest, SVM, or k-NN.
- Use cross-validation for model selection.
- Tune at least one model.
- Report confusion matrix, precision, recall, F1-score, and ROC-AUC where appropriate.
- Address class imbalance if present.
- Recommend one model and justify the choice.

### Mini-Project

**Objective:** Complete an end-to-end machine learning workflow.

**Suggested project themes:**

- Predicting house prices or rental prices
- Student performance prediction
- Customer churn prediction
- Medical risk classification using public datasets
- Sentiment classification using simple text features
- Clustering customer/product profiles
- Detecting anomalies in transactions or sensor readings

**Required deliverables:**

- Project proposal, 1-2 pages
- Cleaned dataset or documented data source
- Reproducible notebook
- Model comparison table
- Short written report, 6-8 pages
- 5-8 minute presentation

**Suggested mini-project rubric:**

| Criterion | Weight |
|---|---:|
| Problem framing and dataset understanding | 15% |
| Data preparation and feature engineering | 20% |
| Model selection and implementation | 20% |
| Evaluation and interpretation | 20% |
| Communication and reproducibility | 15% |
| Ethical reflection and limitations | 10% |

### Final Test/Exam Coverage

- Definitions and ML workflow
- Regression and classification concepts
- Model evaluation and validation
- Overfitting, underfitting, and bias-variance
- Decision trees, random forests, SVMs, clustering, and neural networks
- Metric selection and interpretation
- Practical scikit-learn pipeline reasoning
- Short scenario-based questions

## 7. Teaching Students with Limited ML Background

This course can be taught successfully to students with limited machine learning background by emphasizing intuition before mathematics, using visual explanations, and linking every algorithm to a practical question. Start with familiar examples such as predicting grades, classifying emails, recommending products, or grouping customers. Introduce formulas gradually and connect them to code outputs, plots, and model behavior.

Students should first learn the workflow: define the problem, inspect the data, split the data, train a baseline, evaluate performance, improve carefully, and communicate limitations. Mathematics should be treated as a tool for understanding rather than as a barrier to entry. Short weekly labs are essential because students often understand machine learning best when they can see how changing data, features, parameters, or metrics changes the model result.

Recommended support strategies:

- Begin each topic with a real-world problem and a visual explanation.
- Use small datasets before moving to larger ones.
- Provide starter notebooks with partially completed code.
- Teach one model deeply before comparing many models.
- Revisit the same dataset across several weeks to show workflow continuity.
- Use pair programming or guided lab checkpoints.
- Include brief recap slides on probability, statistics, and linear algebra only when needed.
- Assess both conceptual understanding and practical implementation.
- Reward clear discussion of limitations, not only high accuracy.
- Encourage students to ask: "What data is the model learning from, and what could go wrong?"

## Source Links

- An Introduction to Statistical Learning: https://www.statlearning.com/
- The Elements of Statistical Learning: https://hastie.su.domains/ElemStatLearn/
- scikit-learn User Guide: https://scikit-learn.org/stable/user_guide.html
- Google Machine Learning Crash Course: https://developers.google.com/machine-learning/crash-course
- Mathematics for Machine Learning: https://mml-book.github.io/
- Dive into Deep Learning: https://d2l.ai/
- Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 3rd Edition: https://www.oreilly.com/library/view/hands-on-machine-learning/9781098125967/
- Pattern Recognition and Machine Learning: https://www.microsoft.com/en-us/research/people/cmbishop/prml-book/
