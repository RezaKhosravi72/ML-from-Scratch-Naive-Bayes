## Implementation of Naive Bayes Classifier from Scratch

### Objective: 

Develop a Naive Bayes classifier for classification problems without using external ML libraries. This improves the understanding of probabilistic modeling approaches.

#### Methodology:  

- NaiveBayes class implements classifier functionality in an object-oriented manner.
- The fit() method calculates class priors, mean, and variance to learn Gaussian distributions for each feature.  
- The predict() method evaluates log posteriors by multiplying log priors and log PDF per class to return the predicted class label.
- Data is generated using scikit-learn for evaluation on 1000 samples with 2 classes and 10 features.

### Key aspects:

- **NaiveBayes class** contains methods for fitting the model from training data and predicting new samples.

- fit() method calculates mean, variance, and class priors for each feature dimension per class. This learns the probability distributions. 

- predict() takes the log of posterior probabilities per class and returns the class with the highest probability via argmax(). 

- _predict() calculates posterior as the log of priors multiplied by log PDF (probability density function) of each feature per class.

- PDF uses Gaussian distribution with learned means and variances as it assumes independence between features (naive assumption).

- **Data** for evaluation is generated using sklearn make_classification() with 1000 samples, 2 classes and 10 features. 

- Train test split is done to evaluate held-out data.

- Predictions are made and accuracy is calculated, showing ~96.5% accuracy validating the approach.

#### Evaluation:

- Train-test split is done to validate on held-out data. 
- Accuracy metric is used with 96.5% achieved, showing algorithm effectiveness.

#### Skills:

- Probabilistic modeling concepts
- Implementation of Bayes' theorem for classification  
- NumPy for numeric computing
- Data generation and preprocessing 
- Model evaluation best practices

#### Outcome:
- Intuitive and rigorous implementation establishes a solid understanding of probabilistic algorithms.  
- Successful evaluation of simulated data proves the viability of the from-scratch approach.
- Key probability concepts like density functions, priors, and posteriors are seamlessly integrated.


In conclusion, this project demonstrates capabilities in algorithms, probabilistic modeling, and the ability to build classifiers from the ground up without libraries. A clean, modularized code structure and end-to-end validation approach are showcased. Developing basic machine learning techniques from first principles aids conceptual clarity.
