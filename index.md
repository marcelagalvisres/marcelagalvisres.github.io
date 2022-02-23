## Portfolio

---

### About my projects 

[Project 1 An algorithm to reduce the numer of features in classification using clustering of the categores of categorical predictors](https://marcelagalvisres.github.io/clustcat/)

In this project I developed an algorithm that reduces the number of dummy variables to consider when working with categorical predictors in classification. The algorithm was tested in several real-world datasets from the UCI Machine Learning repository. 

- We significantly reduced the complexity of the model (**60% to 95% reduction** depending on the dataset) in the number of dummies to consider
- Accuracy is preserved or even improved

_Figure 1: Accuracy for the original (not clustered) and clustered model and reduction in complexity for the clustered model_
<img src="images/effect_clust.jpeg?raw=true"/>

---

[Project 2 An algorithms to reduce disparate mistreatment in classification using feature shrinkage](http://example.com/)

In this project, I desgined an algorithm that enhances the trade-off between accuracy and unfairness in classification, by finding a shrunk representation of the features. 
- We optimize that trade-off using a parameter (&alpha;) that determines the weight given to Accuracy
- The main advantage of our approach is that we find a less biased representation of the data, in some cases **even reducing disparate mistreatment to zero** 
- The shrunk representation **does not harm accuracy**

_Figure 2: Accuracy, Unfairness and False Negative Rates for the protected (sex: female) and non-protected (sex: male) group in the Adult dataset using different values of the parameter &alpha;, compared to the original model_
<img src="images/Adult_sex.jpeg?raw=true"/> 


---





---

