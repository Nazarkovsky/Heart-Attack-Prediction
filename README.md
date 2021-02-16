# Heart-Attack-Prediction

## Abstract
The project was prepared and submitted within the Brazilian ["Bootcamp Data Science na prática"](https://www.facebook.com/neuronDSAI/photos/a.1924971354499031/2664668797195946/?type=3&amp;eid=ARCBaznRnMGbE-iFheLbf7HyZpHcxpz7vT-F8J9Yl9_BrqHtwnjLsmdbyaE4l4nbEJKXWdg2aLyGuj7B&amp;ifg=1) by Neuron.

See also [here](https://user-images.githubusercontent.com/63872579/107982816-76e4f180-6fa3-11eb-9ce9-e1abadab44ec.png)

The dataset was provided by the Bootcamp administration [from Kaggle](https://www.kaggle.com/imnikhilanand/heart-attack-prediction). The description of the data is uploaded here as a TXT.

[The certificate](https://user-images.githubusercontent.com/63872579/107994659-d9e28280-6fbb-11eb-80fd-567091e308f8.jpg)

## Methods

In order to perform the typical classification procedure for the binary output, following metrics are required to select the optimal model: misclassification rate or MR, F1, Generalized R2 (Nagelkerke or Craig and Uhler R2), Mean Abs Dev (the average of the absolute values of the differences between the real output and the predicted output). The project is supported by figures found in the Issues section. The information about R2 for classification is [here](https://stats.idre.ucla.edu/other/mult-pkg/faq/general/faq-what-are-pseudo-r-squareds/)

The data were stratified and divided : [75% for training, 25% for validation](https://user-images.githubusercontent.com/63872579/107993039-c71a7e80-6fb8-11eb-92b9-fb462a3de265.jpg).

The models for machine learning: Naive Bayes, K-Nearest Neighbors or KNN (155 Neighbors estimated through euclidean distances at the uniform weights of points), Multiple Logistic Regression, Generalized Regression techniques (Lasso, Elastic Net, Ridge, Double Lasso), SVM (linear kernel function, cost = 1), Classification Tree , Boosted Tree and Bootstrap Forest (10 trees, 3 terms sampled per split, learning rate 0.1).

## Results and Discussions

The most effective trained model was Bootstrap Forest [among other classification models](https://user-images.githubusercontent.com/63872579/108097217-9db52d80-7060-11eb-873e-f72926b957b4.jpg). While [validating](https://user-images.githubusercontent.com/63872579/108101778-795c4f80-7066-11eb-97c0-bf5d8059520d.jpg), it was discovered that majority of models gave MR 7,69% at equal F1 (0.92), whereas their Generaized R2-s were also identical. Thus, among the models, the minimal Mean Abs Dev had the logistic regression. Its Fit data, ROC, confusion matrix are given [here](https://user-images.githubusercontent.com/63872579/108105229-1faa5400-706b-11eb-85ed-b3b5dfb71271.jpg).

As for non-parametric KNN, MR and F1 became higher at the validation at K = 92 (number of neighbors of the minimal MR on validation): MR = 5.77% and F1 = 0.939. See the graphical summary [here](https://user-images.githubusercontent.com/63872579/108113666-8c771b80-7076-11eb-81da-d38959843e33.jpg) and the table of all 155 neighbors vs. MR is found in the uploaded file "KNN-iterations summary by MR.xlsx".

An overall comparison of the values for actual target vs. predicted target by the set models on Validation is [here](https://user-images.githubusercontent.com/63872579/108114487-a107e380-7077-11eb-93ee-7eb7cb36cf04.jpg) and in general is [here](https://user-images.githubusercontent.com/63872579/108114684-e2988e80-7077-11eb-9cee-57dcdb2f5b21.jpg)
