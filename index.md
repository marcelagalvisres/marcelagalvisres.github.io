## Portfolio
---
## Machine Learning Research - Algorithms
## Project 1 
### [An algorithm to reduce the number of features in classification using clustering of the categories of categorical predictors](https://marcelagalvisres.github.io/clustcat/)

- We significantly reduced the complexity (number of dummies to consider) of the logit model **60% to 95% reduction**
- Accuracy is preserved
- See publication available in [Expert Systems with Applications](https://doi.org/10.1016/j.eswa.2021.115245)


_Figure 1: Accuracy for the original and clustered model and reduction in complexity for the clustered model_
<img src="images/effect_clust.jpeg?raw=true"/>

---

## Project 2 
### [An algorithms to reduce disparate mistreatment in classification using feature shrinkage](https://www.researchgate.net/publication/358614960_Improving_fairness_of_Generalized_Linear_Models_by_feature_shrinkage)

- We find a shrunk representation of the features 
- We optimize the trade-off between accuracy and unfairness in classification using a parameter (&alpha;) that determines the weight given to Accuracy when searching for a good shrunk representation
- The main advantage of our approach is that we find a less biased representation of the data, in some cases **even reducing disparate mistreatment to zero** 
- The shrunk representation **does not harm accuracy**
- See preprint: [ResearchGate](https://www.researchgate.net/publication/358614960_Improving_fairness_of_Generalized_Linear_Models_by_feature_shrinkage)

_Figure 2: Accuracy, Unfairness and False Negative Rates for the protected (sex: female) and non-protected (sex: male) group in the Adult dataset using different values of the parameter &alpha;, compared to the original model_
<img src="images/Adult_sex.jpeg?raw=true"/> 

---
## Data Science project 
## Can Machine Learning help reducing costs by better targeting students at risk of dropout?
- I develop prediction models of school dropout using student administration data from Colombia.
- The models **identify correctly between 60% and 80%** of the students who will dropout in the following year, with a **false positive rate between 23% and 32%**
  <img src="images/auc.PNG?raw=true"/> 
- We can _help education authorities target_ their interventions (select groups of students) _to prevent school dropout_
- I assume several scenarios
  - **Scenario 1:** target all students in the highest dropout schools (above 75th percentile) in Grade 6
  - **Scenario 2:** target students with the highest probability of dropping out according to the Gradient Boosting Machines
  - **Scenario 3:** within the schools in scenario 1, target students who have a higher probability of dropping out as estimated with Gradient Boosting Machines

<img src="images/color_blind.png?raw=true"/> 

Prediction algorithms can save up to 24% of the costs associated with an intervention

