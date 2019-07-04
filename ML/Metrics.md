### Metrics
[3.3. Model evaluation: quantifying the quality of predictions — scikit-learn 0.21.2 documentation](https://scikit-learn.org/stable/modules/model_evaluation.html#scoring-parameter)


* Micro-Averaged F1-Score (Mean F Score) : The F1 score can be interpreted as a weighted average of the precision and recall, where an F1 score reaches its best value at 1 and worst score at 0. The relative contribution of precision and recall to the F1 score are equal. The formula for the F1 score is:

F1 = 2 * (precision * recall) / (precision + recall)

In the multi-class and multi-label case, this is the weighted average of the F1 score of each class. 

* 'Micro f1 score': 
Calculate metrics globally by counting the total true positives, false negatives and false positives. This is a better metric when we have class imbalance. 

* 'Macro f1 score': 
Calculate metrics for each label, and find their unweighted mean. This does not take label imbalance into account. 
https://www.kaggle.com/wiki/MeanFScore 
http://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html 

* Hamming loss : The Hamming loss is the fraction of labels that are incorrectly predicted. 
https://www.kaggle.com/wiki/HammingLoss 