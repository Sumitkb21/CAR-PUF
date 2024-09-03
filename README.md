# Companion Arbiter PUF (CAR-PUF) Linear Model Project

## Overview

This project was developed as part of the *Introduction to Machine Learning* course. The primary focus was to analyze the security vulnerabilities of the Companion Arbiter PUF (CAR-PUF) by implementing and comparing linear models using logistic regression and support vector classifiers. The project explored the impact of various hyperparameters on training time and test accuracy, with an emphasis on optimizing model performance and efficiency.

## Project Highlights

- **Model Implementation**: 
  Successfully derived and implemented a linear model using logistic regression that accurately predicts the responses of a Companion Arbiter PUF with an accuracy of 99.3%.

- **Mathematical Derivation**: 
  Provided a mathematical derivation showing that a single linear model can break the security of Companion Arbiter PUFs, demonstrating strong theoretical foundations.

- **Efficiency and Performance**: 
  Reduced the feature vector dimensionality to 528, achieving an error rate of 0.009 and a training time of 14.287 seconds.

## Experimentation with `LinearSVC` and `LogisticRegression`

The project also included a thorough comparison of `sklearn.svm.LinearSVC` and `sklearn.linear_model.LogisticRegression` models. Experiments focused on the impact of various hyperparameters on training time and test accuracy.

### Key Experiments
1. **Regularization Parameter (C)**:
   - Evaluated the effect of setting C to high, medium, and low values in both `LinearSVC` and `LogisticRegression`.
   - Observed how this affects the trade-off between bias and variance, as well as training efficiency.
![image](https://github.com/user-attachments/assets/9e1ce2d6-0481-4754-ad49-82992318ee06)
![image](https://github.com/user-attachments/assets/3f56f638-beac-4d89-a9ff-b78eef9a0f2f)


2. **Tolerance (tol)**:
   - Changed `tol` to high, medium, and low values for both `LinearSVC` and `LogisticRegression`.
   - Measured the impact on convergence time and model performance.
![image](https://github.com/user-attachments/assets/8e2d16c3-7b9f-4ec7-9b90-47b45c6db11e)
![image](https://github.com/user-attachments/assets/5a4b00f5-a98c-44b4-8c3f-4d8b7e065a37)


## Results

- **Accuracy**: 99.3%
- **Error Rate**: 0.007
- **Training Time**: 14.287 seconds
- **Dimensionality**: Reduced feature vector to 528
   
## Conclusion

The project highlights the vulnerabilities of CAR-PUF systems when exposed to linear models like logistic regression and support vector classifiers. Experiments with hyperparameter tuning further demonstrate how different configurations can enhance or hinder model performance. The results underscore the importance of carefully selecting model parameters to balance accuracy and computational efficiency.
