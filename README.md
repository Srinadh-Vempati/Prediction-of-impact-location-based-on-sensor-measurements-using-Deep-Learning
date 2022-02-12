# Prediction-of-impact-location-based-on-sensor-measurements-using-Deep-Learning
To predict the impact location based on the piezo-electric sensor measurements at various impact locations


**Project details:**

- Predict the location of impact using a Deep Learning model trained on the various Numerically and Experimental data sets of sensor measurements (piezo-electric) at various locations.

- Comparison of prediction between DNN and standard ML Regressors.

**Tools:**

Python /  pandas / numpy / scipy / matplotlib / scikit-learn / Tensorflow / keras / Linear Regression / KNeighborsRegressor / DecisionTreeRegressor

**Project Steps:**


**1. Data Preprocessing**

- Numerically Simulated data which spans the sensor measurements for impact locations spanning Quadrant 1.

- Data Augmentation spanning the the rest of the 3 Quadrants was performed.

- Experimental data which contains heavy noise is filtered and preprocessed to mimic the behavior similar to Experimental data


**2. Test-CrossValidation sets genereation**

- Splitting the whole data into Test & Cross-Validation sets.


**3. Machine Learning Regression & Deep Learning Model**

- Regression performed using Mean Absolute Value (MAV) as the feature with 3 standard ML Regressors namely Linear Regressor, Decision Tree Regressor & KNN Regressor.

- 3 individual FFNN models with different architectures (4,5,6 layered nets) have been considered.

-  Optimizing the NN parameters through Hyper-parameter tuning with GridSearch CV method.

- Ensembled prediction over the 3 DL models and optimizing (using gridsearch algorithm in pandas) the final ensembled network.


**Conclusion:**

The Ensembled Network efficiently predicts (lower mse) compared to the ML Regressors.
