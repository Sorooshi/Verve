# Verve DS test



**Objective: Gender classifier using the provided dataset**

Before answering the task's questions, let me explain my point of view of the problem at our hands. In my opinion, instead of determining the gender, a recommender system should track users' preferences, profile their interests, and map their interests to the Ad categories. Anyhow, let me proceed with replying to the questions.

1) Identify 3-5 potential problems you can see with the provided dataset that might make building a classification model difficult.
First of all, the features are not informative enough. More precisely, 
1.1) There is no guarantee that a user uses his/her complete and correct name; thus, using the available APIs/datasets/algorithm, for instance, genderize, would not lead to reliable results.

1.2) Even if the issue mentioned above can be somehow taken care of, to the best of my knowledge, there is no comprehensive dataset containing all languages names, e.g., Arabic, Persian, etc.

1.3) Neither the App category nor the Ad category is not a proper gender identifier, meaning that, depending on a person's personality, characteristics, occupation, etc., he/she might be interested in news, sport, or fashion. 
NB. I agree that some categories of APP/Ad can be somehow more gender-oriented: meaning that the probability of a football game will be more appealing to a boy is far higher than for a girl. Or girls should be more interested in cosmetics than boys (but it still depends on many factors, like culture, countries, occupation, education level, etc.)

1.4) The datasets are highly imbalanced, and clicking on an advertisement rarely happens, making the classification task even harder.


2) Describe briefly how you would find the features that are likely to be the most important for your model.

After proper data splitting and pre-processing, I would decide which evaluation metrics should be used, e,g—accuracy, F1-score, etc. Then I would start by applying various existing models, e.g., Random Forest, training a Neural Network, etc., to choose the best possible model. After selecting the best model, I would apply various feature importance methods, for instance, SHAP methods, to determine the importance of features.

3. Identify which model you would try first and at least one advantage and disadvantage of this choice.
To the best of my experience, the Random Forest (RF) classifier is a pretty robust and powerful algorithm, especially for data sets similar to ours. In short, it has the following pros and cons as follows:
 Pros:
 - works well with non-linear data, 
- lower risk of overfitting. 
- runs efficiently on a large dataset.

Cons:
RFs are found to be biased while dealing with categorical variables.
slow Training.
not suitable for linear methods with a lot of sparse features.




