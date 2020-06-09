#### Question 1: 

<img width="910" alt="Screen Shot 2020-06-08 at 9 58 44 AM (2)" src="https://user-images.githubusercontent.com/55514757/84039318-165ed880-a96f-11ea-9f67-18304afaefa8.png">

`Answer:` 0.52

Explanation: 89 + 72 + 94 + 69 = 324 / 4 = 81 is mean so then 94-81/25 = 0.52

#### Question 2:

You run gradient descent for 15 iterations with α = 0.3 and compute
<sub></sub>J(θ)
after each iteration. You find that the value of
<sub></sub>J(θ)
`decreases slowly` and is still decreasing after 15 iterations. Based on this, which of the following conclusions seem most plausible?

* Rather than use the current value of α, it'd be more promising to try a smaller value of α (say α = 0.1).

* α = 0.3 is an effective choice of learning rate.

* Rather than use the current value of α, it'd be more promising to try a larger value of α (say α = 1.0).

`Answer:` 

Rather than use the current value of α, it'd be more promising to try a smaller value of α (say α = 0.1).

Explanation: A larger value for α should increase the rate of convergence to the minimum of <sub></sub>J(θ)

#### Question 3:

<img width="800" alt="Screen Shot 2020-06-08 at 9 58 13 AM (2)" src="https://user-images.githubusercontent.com/55514757/84039358-224a9a80-a96f-11ea-9566-be7dbbd01ae6.png">

* X is 28 * 5, y is 28 * 1, θ is 5 * 1

* X is 28 * 5, y is 28 * 5, θ is 5 * 5

* X is 28 * 4, y is 28 * 1, θ is 4 * 1

* X is 28 * 4, y is 28 * 1, θ is 4 * 1

`Answer:`

X is 28 * 5, y is 28 * 1, θ is 5 * 1

Explanation: ( m * n ) * ( n * m )

#### Question 4:

Suppose you have a dataset with m = 50m=50 examples and n = 200000n=200000 features for each example. You want to use multivariate linear regression to fit the parameters
<sub></sub>θ
to our data. Should you prefer gradient descent or the normal equation?

* Gradient descent, since 
(X<sup>T</sup>X)^−1
will be very slow to compute in the normal equation.

* The normal equation, since gradient descent might be unable to find the θ.

* Gradient descent, since it will always converge to the optimal θ.

* The normal equation, since it provides an efficient way to directly find the solution.

`Answer:`

Gradient descent, since 
(X<sup>T</sup>X)^−1
will be very slow to compute in the normal equation.

Explanation: With n=200000 features, you will have to invert a 200001×200001 matrix to compute the normal equation. Inverting such a large matrix is computationally expensive, so gradient descent is a good choice.

#### Question 5:

Which of the following are reasons for using feature scaling?

* It speeds up gradient descent by making it require fewer iterations to get to a good solution.

* It is necessary to prevent gradient descent from getting stuck in local optima.

* It speeds up gradient descent by making each iteration of gradient descent less expensive to compute.

* It prevents the matrix X<sup>T</sup>X (used in the normal equation) from being non-invertable (singular/degenerate).

`Answer:`

It speeds up gradient descent by making it require fewer iterations to get to a good solution.

Explanation: Feature scaling speeds up gradient descent by avoiding many extra iterations that are required when one or more features take on much larger values than the rest.
