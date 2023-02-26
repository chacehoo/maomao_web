---
title: Jan 2023 | New paper entitled "Impacts of building load dispersion level on its load forecasting accuracy -  Data or algorithms Importance of reliability and interpretability in machine learning" was published in *Energy and buildings*.

summary: Our recent research paper entitled "**Impacts of building load dispersion level on its load forecasting accuracy - Data or algorithms Importance of reliability and interpretability in machine learning**" was published in *Energy and Buildings*. 

date: 2023-02-26

# View.
#   1 = List
#   2 = Compact
#   3 = Card
view: 2

# Optional header image (relative to `static/img/` folder).
# image in the page of this post; caption is the title of the figure.
header:
  caption: ""   
# image: "renewable_journal.jpg"   
---

The full paper can be found [here](https://doi.org/10.1016/j.enbuild.2023.112896).

Why does Building X have higher forecast accuracy than Building Y? What is the major factor contributing to the high forecast accuracy of Building X? DATA or ALGORITHMS? Regarding DATA, what building load characteristics affect the forecast accuracy and how can we quantify this influential factor? Regarding ALGORITHMS, what algorithms are more likely to outperform others in the field of building load forecasting? Do deep learning models outperform conventional "shallow" machine learning models? What model is the feasible model for benchmarking?
 
To shed some light on these questions and improve the RELIABILITY and INTERPRETABILITY of ML techniques, we examined the impacts of building load dispersion level on its best load forecasting accuracy. This was accomplished by comparing the performances of 11 different prediction models, including “shallow” machine learning and deep learning techniques, over 9 weeks of operation for 56 British non-domestic buildings. Two key takeaways are:

* Each building has its best achievable forecasting performance and most importantly, it is largely influenced by its load dispersion level. In our study, we proposed novel metrics to quantify the dispersion level of building intraday load profiles.

* There is not a panacea-like individual model for all building load forecasting problems. A complex model structure does not guarantee a higher forecasting performance. We find that conventional “shallow” ML models still outperform the increasingly popular deep learning models for time-series load forecasting. We also demonstrate that the naive persistent model is not naive at all after a long period of testing and it is recommended to be used as the benchmarking model in the building load forecasting problem.

Thrilled to see my last piece of work at Oxford finally coming out. Many thanks to our co-authors without whom it would not be possible to put together this work: Bruce Stephen, Jethro Browell, Stephen Haben, and David Wallom.

