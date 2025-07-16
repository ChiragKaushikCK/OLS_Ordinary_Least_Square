# OLS_Ordinary_Least_Square

<h2 id="ols-explanation-section" style="color: #333; font-family: 'Segoe UI', sans-serif; font-size: 2.5em; border-bottom: 3px solid #FFC107; padding-bottom: 10px;">
  💡 Understanding Ordinary Least Squares (OLS)
</h2>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  **Ordinary Least Squares (OLS)** is a fundamental method used in linear regression for estimating the unknown parameters (coefficients) of a linear model. Its primary goal is to find the line (or hyperplane in the case of multiple regression) that best fits the given data.
</p>
<h3 style="color: #28A745; font-size: 1.8em; margin-top: 25px;">How OLS Works:</h3>
<p style="font-size: 1.1em; color: #444; line-height: 1.6;">
  At its core, OLS works by minimizing the **sum of the squares of the residuals**. A residual is the difference between an observed value (actual data point) and the value predicted by the regression line.
</p>
<p align="center" style="font-size: 1.3em; font-weight: bold; color: #28A745; margin: 20px 0;">
  $$ \text{Minimize} \sum_{i=1}^{n} (Y_i - \hat{Y}_i)^2 $$
</p>
<ul style="list-style-type: none; padding: 0; font-size: 1.1em; color: #444;">
  <li style="margin-bottom: 10px; background-color: #F0FFF0; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #28A745;">$Y_i$:</strong> The observed (actual) value of the dependent variable for the $i$-th data point.
  </li>
  <li style="margin-bottom: 10px; background-color: #F0FFF0; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #28A745;">$\hat{Y}_i$:</strong> The predicted value of the dependent variable by the regression model for the $i$-th data point.
  </li>
  <li style="margin-bottom: 10px; background-color: #F0FFF0; padding: 10px 15px; border-radius: 8px; box-shadow: 0 1px 5px rgba(0,0,0,0.05);">
    <strong style="color: #28A745;">$(Y_i - \hat{Y}_i)$:</strong> The residual for the $i$-th data point.
  </li>
</ul>
<p style="font-size: 1.1em; color: #444; line-height: 1.6; margin-top: 15px;">
  By squaring the differences, OLS ensures that both positive and negative residuals contribute to the sum, and larger errors are penalized more heavily. The coefficients that result in the smallest sum of squared residuals are considered the "best" estimates for the linear model.
</p>
<h3 style="color: #28A745; font-size: 1.8em; margin-top: 25px;">Why Use OLS?</h3>
<ul style="list-style-type: disc; padding-left: 20px; font-size: 1.1em; color: #444;">
  <li><strong style="color: #28A745;">Simplicity:</strong> It's conceptually straightforward and computationally efficient.</li>
  <li><strong style="color: #28A745;">Interpretability:</strong> The resulting coefficients are easy to interpret, representing the change in the dependent variable for a one-unit change in the independent variable (holding others constant in multiple regression).</li>
  <li><strong style="color: #28A745;">Statistical Properties:</strong> Under certain assumptions (e.g., linearity, independence of errors, homoscedasticity, normality of errors), OLS estimators are the Best Linear Unbiased Estimators (BLUE), meaning they have the smallest variance among all linear unbiased estimators.</li>
</ul>

