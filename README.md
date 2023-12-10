# Comparing-XGBoost-and-CATBoost
The dynamics of XGBoost and CatBoost in a comprehensive classification project, evaluating their adaptability to normal, scaled, PCA, LDA, and Kernel PCA-transformed features. Finding the performance variations, providing valuable insights for feature engineering and algorithm selection in machine learning classification tasks.

**Overview:**
Explore the effectiveness of XGBoost and CatBoost algorithms across varied feature sets—normal, scaled, PCA, LDA, and Kernel PCA. This GitHub repository provides a comprehensive analysis to guide optimal feature engineering and algorithm selection for classification tasks. Contribute, learn, and elevate your data science projects.

**Key Features:**
- Comparative analysis of XGBoost and CatBoost
- Diverse feature sets: normal, scaled, PCA, LDA, Kernel PCA
- Accurate classification insights
- Interactive Jupyter notebooks for experimentation
- Easy-to-follow code structure and documentation

**Usage:**
1. Clone the repository
2. Explore Jupyter notebooks for detailed analyses
3. Experiment with different datasets and feature engineering techniques
4. Contribute enhancements and insights

**Contributions:**
Contributions are welcome! Open issues, provide feedback, or submit pull requests to enhance this collaborative resource.

**Tools and Libraries:**
- XGBoost, CatBoost, NumPy, Pandas, Matplotlib, Scikit-learn

# Findings 

Analyzing the results from XGBoost and CatBoost across different feature engineering techniques provides valuable insights:

1. **Normal Features:**
   - **XGBoost:** 96.71%, CatBoost: 97.26%
   - CatBoost slightly outperforms XGBoost in accuracy on the original feature set.
   - Both models exhibit similar performance with minimal deviation.

2. **Scaled Features:**
   - **XGBoost:** 96.71%, CatBoost: 97.26%
   - Scaled features maintain the same performance as normal features for both models.
   - Feature scaling does not significantly impact model accuracy in this case.

3. **Features Extracted via PCA:**
   - **XGBoost:** 96.88%, CatBoost: 97.06%
   - Both models achieve slightly improved accuracy compared to normal features.
   - PCA demonstrates a positive impact on model performance.

4. **Features Extracted via LDA:**
   - **XGBoost:** 97.07%, CatBoost: 97.07%
   - Both models show enhanced accuracy compared to the original and scaled features.
   - Linear Discriminant Analysis (LDA) is effective in capturing relevant information.

5. **Features Extracted via K-PCA:**
   - **XGBoost:** 94.87%, CatBoost: 95.78%
   - Both models experience a decrease in accuracy compared to other feature sets.
   - Kernel PCA introduces non-linearity that may not benefit the models in this context.

**Conclusion:**
- CatBoost consistently demonstrates slightly higher accuracy than XGBoost across all feature sets.
- Feature scaling has a minimal impact on both models.
- PCA and LDA contribute positively to model accuracy.
- Kernel PCA may not be as effective in this context, resulting in a decrease in accuracy.

The choice between XGBoost and CatBoost depends on the specific requirements of the problem and the significance of computational efficiency, as CatBoost generally performs well "out of the box" without extensive tuning. Consideration of these results aids in selecting the most suitable model and feature engineering strategy for the given dataset.
