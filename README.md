Surrogate Modeling Benchmark for Data-Efficient Experiments
Overview

This project evaluates the performance of different surrogate modeling techniques for predicting outcomes of high-dimensional systems when experimental data is scarce.

In many real-world engineering systems—such as semiconductor manufacturing processes—running experiments can be expensive and time-consuming. Instead of performing a large number of experiments, surrogate models can approximate the relationship between input variables and system outputs using a limited dataset.

This project benchmarks several machine learning models to study how efficiently they learn from small datasets.

Objective

The goal of this project is to:

Compare different surrogate modeling methods
Evaluate their prediction accuracy under limited data
Analyze sample efficiency as the training dataset grows
Understand which models are most suitable for high-dimensional experimental systems

Methods

The experiment uses a synthetic benchmark function (Ackley function) to simulate a complex system where each evaluation represents an expensive experiment.

Workflow

Generate synthetic high-dimensional data
Split data into training and testing sets
Train surrogate models using varying training sample sizes
Evaluate prediction accuracy on unseen data
Compare model performance using Mean Squared Error (MSE)

Models Evaluated

The following surrogate models were benchmarked:

Polynomial Regression (Response Surface Model)
Random Forest Regression
Support Vector Regression (SVR)
Gaussian Process Regression (GPR)

Gaussian Process models are commonly used in Bayesian optimization and experimental design because they provide uncertainty estimates along with predictions.

Key Concepts

This project explores several important ideas used in modern experimental modeling:

Surrogate Modeling
Design of Experiments (DOE)
Data-efficient machine learning
High-dimensional optimization
Sample efficiency analysis

These techniques are widely used in fields such as:
Semiconductor process optimization
engineering simulations
Materials discovery
Scientific machine learning

Tools and Libraries

The project was implemented using:

Python
NumPy
Pandas
Scikit-learn
Matplotlib
Google Colab

Results

Model performance was evaluated by measuring test error across different training dataset sizes.

The results illustrate how different surrogate models perform under data scarcity, highlighting the importance of model choice in expensive experimental systems.
