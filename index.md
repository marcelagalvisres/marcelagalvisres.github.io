## Portfolio
## Data Science- Can Machine Learning help reducing the costs of public interventions by better targeting students at risk of dropout?
- I develop prediction models (Random Forests RF, Gradient Boosting Machines GBM, Logistic Regression LR) of school dropout using student administration data from Colombia.
- The models **identify correctly between 60% and 80%** of the students who will dropout in the following year, with a **false positive rate between 23% and 32%**
  <img src="images/auc.PNG?raw=true"/> 
- The models **can help education authorities target** their interventions by better selecting groups of students **with a high probability of dropout**
- Assume three scenarios
  - **Scenario 1:** target _all students in the highest dropout schools_ (above 75th percentile)
  - **Scenario 2:** target _students with the highest probability_ of dropping out according to the Gradient Boosting Machines
  - **Scenario 3:** _within the schools in scenario 1, target students who have a higher probability_ of dropping out as estimated with Gradient Boosting Machines

<img src="images/color_blind.png?raw=true"/> 

- I compare these scenarios in terms of their **cost effectiveness** (cost per student retained) and **benefits** (lifetime earnings for a high school gradute)
- The plot shows that the Prediction algorithms _can save up to 24% of the costs_ associated with an educational intervention

---
## Algorithms - Optmizing interpretability and fairness of machine learning models 
### [An algorithm to reduce the number of features in classification using clustering of the categories of categorical predictors](https://marcelagalvisres.github.io/clustcat/)

- We significantly reduced the complexity (number of dummies to consider) of the logit model **60% to 95% reduction**
- Accuracy is preserved
- See publication available in [Expert Systems with Applications](https://doi.org/10.1016/j.eswa.2021.115245)


_Figure 1: Accuracy for the original and clustered model and reduction in complexity for the clustered model_
<img src="images/effect_clust.jpeg?raw=true"/>

---

### [An algorithms to reduce disparate mistreatment in classification using feature shrinkage](https://www.researchgate.net/publication/358614960_Improving_fairness_of_Generalized_Linear_Models_by_feature_shrinkage)

- We find a shrunk representation of the features 
- We optimize the trade-off between accuracy and unfairness in classification using a parameter (&alpha;) that determines the weight given to Accuracy when searching for a good shrunk representation
- The main advantage of our approach is that we find a less biased representation of the data, in some cases **even reducing disparate mistreatment to zero** 
- The shrunk representation **does not harm accuracy**
- See preprint: [ResearchGate](https://www.researchgate.net/publication/358614960_Improving_fairness_of_Generalized_Linear_Models_by_feature_shrinkage)

_Figure 2: Accuracy, Unfairness and False Negative Rates for the protected (sex: female) and non-protected (sex: male) group in the Adult dataset using different values of the parameter &alpha;, compared to the original model_
<img src="images/Adult_sex.jpeg?raw=true"/> 



