---
{"dg-publish":true,"permalink":"/Mainfolder/Statistics/Regression/"}
---

## What is linear regression
>**Regression**: Technique to model linear relationships between two quantitative variables.  
>**Goal**: Predict values of a response variable (dependent) using an explanatory variable (independent/predictor).  


**Equations:**
  - Statistics notation:  
    $\hat{y} = \beta_0 + \beta_1X$  
    - $\beta_1$: Slope (change in $y$ per unit change in $x$).  
    - $\beta_0$: Intercept (predicted $y$ when $x = 0$).  
  - Example: Predicting son's height ($\hat{y}$) from father's height ($X$):  
    $\hat{y} = 33.893 + 0.514X$  

---
## 2. Key Calculations  
- Slope ($\beta_1$):  
  $\beta_1 = \left( \frac{s_y}{s_x} \right) r$  
  - $s_x, s_y$: Standard deviations of $x$ and $y$.  
  - $r$ [[Pearson's Correlation Coefficient\|Pearson's Correlation Coefficient]].  
  - Example: For father-son heights:  
    $\beta_1 = \left( \frac{2.81}{2.74} \right) \times 0.501 = 0.514$  

- Intercept ($\beta_0$):  
  $\beta_0 = \bar{y} - \beta_1 \bar{x}$  
  - Example:  
    $\beta_0 = 68.68 - 0.514 \times 67.68 = 33.893$  

---

## 3. Residuals & Model Fit  
- Residual ($e$):  
  $e = y - \hat{y}$  
  - Interpretation:  
    - **Positive** $e$: Underpredicted value.  
    - **Negative** $e$: Overpredicted value.  
  - Example: Father's height = 65 inches → Predicted son's height = 67.30 inches. Observed son's height = 59.8 inches:  
    $e = 59.8 - 67.30 = -7.5$  
    *Interpretation: Overpredicted by 7.5 inches.*  

- Quality of Fit:  
  - $R^2$ (Coefficient of Determination):  
    $R^2 = \frac{\text{Variance of predicted } y}{\text{Variance of observed } y} = r^2$  
    - Interpretation: % of variation in $y$ explained by $x$.  
    - Example: $r = 0.501$ → $R^2 = 0.251$.  
      *25.1% of son's height variation explained by father's height.*  

---

## 4. Assumptions & Pitfalls  
1. Linearity: Relationship must be approximately linear (verify with scatterplot).  
2. Extrapolation: Avoid predictions outside the observed data range.  
   - Example: Predicting son's height for a father with 0 inches is nonsensical.  
3. Correlation ≠ Causation: High $R^2$ does not imply $x$ causes $y$.  
4. Outliers: Can disproportionately affect slope and intercept.  

---

## 5. Comparison with Correlation  

| Aspect       | Correlation ($r$) | Regression |  
|-------------------|---------------------------|----------------|  
| Symmetry          | Symmetric ($r_{xy} = r_{yx}$) | Asymmetric (switching $x$ and $y$ changes the line) |  
| Units             | Unitless                  | Slope has units ($y$-units per $x$-unit) |  
| Purpose           | Measures association      | Predicts $y$ from $x$ |  

## 7. Complementary Tools  
- Scatterplots: Visualize linearity, strength, direction, and outliers.  
- Robust Measures:  
  - [[Mainfolder/Statistics/Spearman's rank correlation\|Spearman's rank correlation]] $\rho$: Use for monotonic but non-linear relationships.  
  - Order Statistics (Median, IQR): Describe skewed data or outliers.  

## Multiple Linear Regression (MLR)

MLR extends simple linear regression by incorporating multiple independent variables to predict a single dependent variable.

### Key Components:
- Model equation: $Y = \beta_0 + \beta_1X_1 + \beta_2X_2 + ... + \beta_pX_p + \varepsilon$
- Partial regression coefficients: Effect of each $X$ on $Y$ while holding other variables constant

### Key Measures:
- Multiple $R^2$: Total variance explained by all predictors
- Adjusted $R^2$: Accounts for the number of predictors (penalizes overfitting)
- F-statistic: Tests overall significance of the model
- t-statistics: Test significance of individual predictors

### Advanced Concepts:
- Multicollinearity: Correlation among predictors
- VIF (Variance Inflation Factor): Detects multicollinearity
- Standardized coefficients (Beta): Compare predictors with different scales
- Interaction effects: When the effect of one predictor depends on another
- Polynomial regression: Adding higher-order terms ($X^2$, $X^3$, etc.)

## Regression Error Analysis

Regression error refers to the discrepancy between observed values and those predicted by the regression model.

### Key Error Metrics:
- Residuals: $e = Y - \hat{Y}$ (observed minus predicted values)
- Mean Squared Error (MSE): Average of squared residuals
- Root Mean Squared Error (RMSE): Square root of MSE, in same units as $Y$
- Mean Absolute Error (MAE): Average of absolute residuals
- Residual Sum of Squares (RSS or SSE): $\sum(Y - \hat{Y})^2$

### Diagnostic Tools:
- Residual plots: Visual check for patterns in residuals
- Q-Q plots: Assess normality of residuals
- Cook's distance: Identify influential observations
- Leverage: Measure of how far an observation is from others in X-space
- DFFITS and DFBETAS: Measure influence of observations on model

### Common Error Issues:
- Heteroscedasticity: Non-constant variance of errors
- Autocorrelation: Correlation among residuals
- Non-normality: When residuals don't follow normal distribution
- Specification error: Incorrect functional form of model

### Model Validation:
- Cross-validation: Testing model performance on unseen data
- Train-test split: Divided dataset for model building and validation
- k-fold cross-validation: Repeatedly partition data for robust validation

## Connections Between ANOVA and Regression

- ANOVA as a special case of regression: Categorical predictors in regression are equivalent to ANOVA
- Regression ANOVA table: Partitions variance similar to traditional ANOVA
- F-test in regression: Tests overall model significance using ANOVA principles

