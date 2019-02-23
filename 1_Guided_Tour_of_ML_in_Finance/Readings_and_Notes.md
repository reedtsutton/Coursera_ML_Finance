### I. Goodfellow, Y. Bengio, A. Courville, “Deep Learning”, 

#### Chapter 4.5 


#### Chapter 5.1, 5.2, 5.3, 5.4


### Leo Breiman, “Statistical Modeling: The Two Cultures” (http://www2.math.uu.se/~thulin/mm/breiman.pdf)  
- Two cultures in statistical modeling to produce or reach conclusions; (1) stochastic models (assuming randomly generated data according to a probability distribution- think traditional statistics), and (2) algorithmic modelling that disregards the data generating mechanism.
- 98% of statisticians use (1), but many people use (2) for applying statistics to other field, and industry. This is what most ML falls into as well.
- When a model is fit to data to draw quantitative conclusions: * The conclusions are about the model's mechanism, and not about nature's mechanism. It follows that: * If the model is a poor emulation of nature, the conclusions may be wrong.
- Goodness of fit tests lack power to detect goodness of fit in more than 3 dimensions - this is from one of the fathers of residual analysis (William Cleveland). As well, residual plot analysis is deeply flawed and limited in cases of many dimensions especially. 
- Simple parametric models imposed on data from complex systems , produces much lower accuracy than algorithmic models. 
- More complex data models are starting to appear in publications, such as Bayesian methods, Markov Chain Monte Carlo. 
- Only one assumption in algorithmic modeling theory; data is drawn independent and identically distributed, from an unknown multivariate distribution. There is lack of theory for many algorithms. Eg. boosting, very good for forming ensembles, but no finite sample size theory that explains why it works so well. 
- Support vector machines have proved to be, in many cases, more accurate predictors in classification and regression than neural nets. 
- Multiplicity problem (Rashomon Effect): The picture of which covariates are important can vary significantly between two models having the same deviance. Model can become unstable when you remove covariates, depending on which ones you remove. Solution is bagging or ensembling in ML!
- Single trees, easily interpretable, B+ in prediction, Forests of trees, A+ in prediction, but suffer lower interpretability. 
- Trying to choose between accuracy and interpretability is not always the right question. The goal of statistical analysis is accurate information, not interpretable information. Random forests can give more reliable information about covariates strengths, even if they don't give much information about how those covariates produce the response. 
- Instead, a new paradigm is that, higher predictive accuracy is associated with more reliable information about the underlying data mechanism, whereas low predictive accuracy can lead to questionable conclusions. Algorithmic models give better predictive accuracy. 
