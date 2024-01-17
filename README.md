## Mushroom Predictor

Welcome to a comprehensive data science project delving into the intriguing realm of fungi—specifically, mushrooms. These fungal entities boast a spectrum of characteristics, ranging from the culinary allure of edibility to the potential dangers of toxicity. The fundamental premise that every mushroom is inherently edible introduces a caveat, highlighting a subset that is consumable only once, underscoring the importance of accurate identification to prevent inadvertent accidents.

![mushroom_image](images/others/mush.jpg)

In the context of this project, our primary objective is to leverage a dataset encompassing various mushroom characteristics. Through advanced data science methodologies, we aim to develop a predictive model capable of discerning whether a given mushroom is likely to be poisonous or not. The analysis includes the use of advanced data science methodologies such as permutance importances, SHAP values, and partial dependence plots.

 This predictive endeavor holds paramount significance, offering a proactive solution for enthusiasts, foragers, and researchers alike. By harnessing the power of machine learning and statistical analysis, we aspire to enhance our understanding of mushroom toxicity, contributing to a safer and more informed exploration of these fascinating fungal entities.

This project was inspired by the article https://towardsdatascience.com/shap-for-categorical-features-7c63e6a554ea


## Data Import and Preprocessing
The initial step involves importing data from the UCI Machine Learning Repository and exploring the dataset. Mushroom characteristics are crucial in evaluating potential toxicity. Features are segregated from the target variable, and the data is split into training and testing sets.

- Variable Encoding: Categorical variables are encoded using One-Hot Encoding to make them understandable for machine learning algorithms. The 'poisonous' class is binary-encoded as 0 (edible) or 1 (poisonous).

- Model Training: The Random Forest algorithm is chosen to make predictions on the toxicity of mushrooms. A classification report is generated to assess the model's performance, indicating high accuracy of 98%.

- Permutance Importances: Permutation importances highlight the variables that significantly influence the model's predictions. "Odor," "gill-size," and "spore-print-color" stand out as pivotal features.

- Partial Dependence Plots: Partial dependence plots reveal the relationship between specific features and the model's predictions. Variables like "odor" and "gill size" exhibit substantial influence on the model's decisions.

- SHAP Values Analysis: SHAP values offer insights into the importance and impact of individual features on model predictions. Odor features, gill size, and color are identified as decisive factors influencing the model's output.

## Conclusion
- Model Accuracy: The model demonstrates a notable accuracy of 98%.

- Mushroom toxicity is closely associated with inherent characteristics influenced by factors like spore color and odor.

- Consistency Across Analyses: Consistency across different analyses confirms the pivotal role of certain variables, particularly odor and gill-size, in shaping the model's decisions.

- *Consulting expert sources is recommended for a more comprehensive understanding.*