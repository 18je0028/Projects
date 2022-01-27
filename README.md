Implement class SGDRegressor. Specification:

class is inherited from sklearn.base.BaseEstimator

constructor takes parameters eta – gradient step (10−3 by default) and n_epochs – dataset pass count (3 by default)

constructor also creates mse_ and weights_ lists in order to track mean squared error and weight vector during gradient descent iterations

Class has fit and predict methods

The fit method takes matrix X and vector y (numpy.array objects) as parameters, appends column of ones to X on the left side, initializes weight vector w with zeros and then makes n_epochs iterations of weight updates (you may refer to this article for details), and for every iteration logs mean squared error and weight vector w in corresponding lists we created in the constructor.

Additionally the fit method will create w_ variable to store weights which produce minimal mean squared error

The fit method returns current instance of the SGDRegressor class, i.e. self

The predict method takes X matrix, adds column of ones to the left side and returns prediction vector, using weight vector w_, created by the fit method.
