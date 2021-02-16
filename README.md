# Heart-Attack-Prediction

## Abstract
The project was prepared and submitted within the Brazilian ["Bootcamp Data Science na prática"](https://www.facebook.com/neuronDSAI/photos/a.1924971354499031/2664668797195946/?type=3&amp;eid=ARCBaznRnMGbE-iFheLbf7HyZpHcxpz7vT-F8J9Yl9_BrqHtwnjLsmdbyaE4l4nbEJKXWdg2aLyGuj7B&amp;ifg=1) by Neuron.

See also [here](https://user-images.githubusercontent.com/63872579/107982816-76e4f180-6fa3-11eb-9ce9-e1abadab44ec.png)

The dataset was provided by the Bootcamp administration [from Kaggle](https://www.kaggle.com/imnikhilanand/heart-attack-prediction)

[The certificate](https://user-images.githubusercontent.com/63872579/107994659-d9e28280-6fbb-11eb-80fd-567091e308f8.jpg)

## Methods

In order to perform the typical classification procedure for the binary output, following metrics are required to select the optimal model: misclassification rate, F1, Generalized R2 (Nagelkerke or Craig and Uhler R2), Mean Abs Dev (the average of the absolute values of the differences between the response and the predicted response). The project is supported by figures found in the Issues section. The information about R2 for classification is [here](https://stats.idre.ucla.edu/other/mult-pkg/faq/general/faq-what-are-pseudo-r-squareds/)

The data were stratified and divided : [75% for training, 25% for validation](https://user-images.githubusercontent.com/63872579/107993039-c71a7e80-6fb8-11eb-92b9-fb462a3de265.jpg).

The models for machine learning: Naive Bayes, K-Nearest Neighbors (155 Neighbors estimated through euclidean distances at the uniform weights of points), Multiple Logistic Regression, Generalized Regression techniques (Lasso, Elastic Net, Ridge, Double Lasso), SVM (linear kernel function, cost = 1), Boosted Tree and Bootstrap Forest.

## Results and Discussions


