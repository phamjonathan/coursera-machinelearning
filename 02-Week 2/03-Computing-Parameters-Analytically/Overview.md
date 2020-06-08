## Normal Equation

`Note`: [8:00 to 8:44 - The design matrix X (in the bottom right side of the slide) given in the example should have elements x with subscript 1 and superscripts varying from 1 to m because for all m training sets there are only 2 features
<sub></sub>x
<sub>0</sub>
and
<sub></sub>x
<sub>1</sub>.
12:56 - The X matrix is m by (n+1) and NOT n by n. ]

Gradient descent gives one way of minimizing J. Let’s discuss a second way of doing so, this time performing the minimization explicitly and without resorting to an iterative algorithm. In the "Normal Equation" method, we will minimize J by explicitly taking its derivatives with respect to the
<sub></sub>θ
<sub>j</sub>
and setting them to zero. This allows us to find the optimum theta without iteration. The normal equation formula is given below:

<img width="155" alt="Screen Shot 2020-06-07 at 11 39 48 PM" src="https://user-images.githubusercontent.com/55514757/83990652-5cd51880-a918-11ea-8b70-8b9ee527c661.png">

<img width="580" alt="Screen Shot 2020-06-07 at 11 39 53 PM" src="https://user-images.githubusercontent.com/55514757/83990658-5fd00900-a918-11ea-9a64-c62a21b203dd.png">

There is `no need` to do feature scaling with the normal equation.

The following is a comparison of gradient descent and the normal equation:

<img width="565" alt="Screen Shot 2020-06-07 at 11 42 18 PM" src="https://user-images.githubusercontent.com/55514757/83990783-c0f7dc80-a918-11ea-8ee4-3bddbc2ba390.png">

## Normal Equation Noninvertibility

<img width="525" alt="Screen Shot 2020-06-07 at 11 46 23 PM" src="https://user-images.githubusercontent.com/55514757/83990932-3663ad00-a919-11ea-994e-b4a0fdfa3bd7.png">


* Redundant features, where two features are very closely related (i.e. they are linearly dependent)

* Too many features (e.g. m ≤ n). In this case, delete some features or use "regularization" (to be explained in a later lesson).

Solutions to the above problems include deleting a feature that is linearly dependent with another or deleting one or more features when there are too many features.