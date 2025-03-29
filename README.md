# Wine-Quality-Prediction

### Abstract

To predict the quality for white and red wines, we applied Generalized Linear Models (GLM), Generalized Additive Models (GAM), Gaussian Mixture Models (GMM) and Random Forest modeling to identify the best-fitting approach. Both GLM and GMM were found to be ineffective in this context. Evaluation results indicated that both the GAM with a Gamma distribution and the Random Forest classifier demonstrated the strongest predictive power. The GAM with Gamma distribution yielded the lowest Akaike Information Criterion (AIC) scores (red wine: 2526.03; white wine: 8654.79) and the lowest misclassification rates (red wine: ~39.0%; white wine: ~46.0%). The Random Forest classifier achieved notable accuracy levels for both varieties (red wine: 65.00%; white wine: 71.12%). Our analysis highlighted the significant role of the `alcohol` feature in predicting wine quality for both white and red wines, followed by `density`, `volatile acidity`, `sulphates`, and `total sulfur dioxide`. Our process also identified challenges related to outlier sensitivity and complex interactions between features.

### Scientific Hypotheses

**Physicochemical Properties Predict Wine Quality**

- Statement: The physicochemical properties of wines, such as acidity, alcohol content, and sulfur dioxide levels, can predict the distribution of wine quality on a scale from 0 (very poor) to 10 (excellent).
- Rationale: Wine quality is influenced by a complex interplay of various physicochemical properties. Previous studies have shown that factors like acidity, alcohol content, and sulfur dioxide levels play crucial roles in determining the sensory attributes of wine. By analyzing these properties, we aim to build predictive models that can estimate the quality distribution for new wine samples.

**Differences in Physicochemical Properties Between Red and White Wines Influence Quality**

- Statement: There are significant differences in the physicochemical properties between red and white wines.
- Rationale: Red and white wines are produced using different processes, which can lead to distinct chemical compositions. These differences can affect the sensory attributes and, consequently, the perceived quality of the wines. By comparing the physicochemical properties of red and white wines, we aim to understand how production methods and chemical composition impact wine quality.

**Certain Physicochemical Features are More Strongly Correlated with Wine Quality**

- Statement: Specific physicochemical features are more strongly correlated with wine quality than others and contribute significantly to the perceived quality of wine.
- Rationale: Not all physicochemical properties may have an equal impact on wine quality. Some features might have a stronger influence on the sensory attributes that determine quality. By identifying the most influential features, we can provide insights into which properties are critical for improving wine quality. 


### Conclusion

**Hypothesis Conclusions**

Our findings support the hypothesis that physicochemical properties such as alcohol content, density, and volatile acidity significantly predict wine quality. The importance of these features varies between white and red wines, indicating that different properties influence the prediction model of each wine type.

The analysis confirms significant differences in physicochemical properties between red and white wines. These differences are crucial for understanding how production methods and chemical composition impact wine quality.

Specific physicochemical features are more strongly correlated with wine quality than others. For white wines, alcohol content, density, and volatile acidity are most influential, while for red wines, alcohol content, sulphates, and total sulfur dioxide are key predictors.

**Important Variables**

The most influential feature for both white and red wines is `alcohol`, highlighting its critical role in determining wine quality. For white wine, `density` and `volatile acidity` are important, suggesting their impact on sensory attributes. For red wine, `sulphates` and `total sulfur dioxide` are significant, likely due to their effects on sensory attributes and preservation.

**Most Appropriate Model**
	
For predicting the distribution of wine quality, the GAM with the Gamma family is the most appropriate model, offering the best balance between model complexity and goodness of fit. If the focus is on classification without needing the distribution, the Random Forest model is the best choice, providing high accuracy and feature importance insights.

