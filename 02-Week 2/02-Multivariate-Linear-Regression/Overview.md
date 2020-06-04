## Multiple Features

<img width="468" alt="Screen Shot 2020-06-02 at 11 05 23 PM" src="https://user-images.githubusercontent.com/55514757/83591412-da1e1900-a525-11ea-88e9-e7a709566847.png">

Linear regression with multiple variables is also known as "`multivariate linear regression`".

We now introduce notation for equations where we can have any number of input variables.

<img width="345" alt="Screen Shot 2020-06-02 at 11 08 18 PM" src="https://user-images.githubusercontent.com/55514757/83591506-1782a680-a526-11ea-91f6-5d7ef378a497.png">

The multivariable form of the hypothesis function accommodating these multiple features is as follows:

<img width="342" alt="Screen Shot 2020-06-02 at 11 10 49 PM" src="https://user-images.githubusercontent.com/55514757/83591654-6cbeb800-a526-11ea-8390-073646a4b458.png">

In order to develop intuition about this function, we can think about 
<sub></sub>θ
<sub>0</sub>
as the basic price of a house, 
<sub></sub>θ
<sub>1</sub>
as the price per square meter,
<sub></sub>θ
<sub>2</sub>
as the price per floor, etc.
<sub></sub>x
<sub>1</sub>
will be the the number of square meters in the house, 
<sub></sub>x
<sub>2</sub>
the number of floors, etc.

Using the definition of matrix multiplication, our multivariable hypothesis function can be concisely represented as:

<img width="348" alt="Screen Shot 2020-06-02 at 11 17 12 PM" src="https://user-images.githubusercontent.com/55514757/83592016-5e24d080-a527-11ea-84eb-26422b9fece2.png">

This is a vectorization of our hypothesis function for one training example; see the lessons on vectorization to learn more.

<img width="545" alt="Screen Shot 2020-06-02 at 11 20 22 PM" src="https://user-images.githubusercontent.com/55514757/83592178-c2e02b00-a527-11ea-9e79-9acc4637df6c.png">

## Gradient Descent For Multiple Variables

### Gradient Descent for Multiple Variables

The gradient descent equation itself is generally the same form; we just have to repeat it for our 'n' features:

<img width="300" alt="Screen Shot 2020-06-03 at 9 07 00 AM" src="https://user-images.githubusercontent.com/55514757/83640401-12e7dd80-a57a-11ea-8837-c20f74e25395.png">

In other words:

<img width="400" alt="Screen Shot 2020-06-03 at 9 08 54 AM" src="https://user-images.githubusercontent.com/55514757/83640407-154a3780-a57a-11ea-849e-7d4422463740.png">

The following image compares gradient descent with one variable to gradient descent with multiple variables:

<img width="620" alt="Screen Shot 2020-06-03 at 9 09 42 AM" src="https://user-images.githubusercontent.com/55514757/83640424-19765500-a57a-11ea-87aa-edb70a717a13.png">

## Gradient Descent in Practice I - Feature Scaling

`Note:` [6:20 - The average size of a house is 1000 but 100 is accidentally written instead]

We can speed up gradient descent by having each of our input values in roughly the same range. This is
<sub></sub>θ
will descend quickly on small ranges and slowly on large ranges, and so will oscillate inefficiently down to the optimum when the variables are very uneven.

The way to prevent this is to modify the ranges of our input variables so that they are all roughly the same. Ideally:

-1 ≤ 
<sub></sub>x
<sub>(i)</sub>
≤ 1

or

-0.5 ≤
<sub></sub>x
<sub>(i)</sub>
0.5

These aren't exact requirements; we are only trying to speed things up. The goal is to get all input variables into roughly one of these ranges, give or take a few.

Two techniques to help with this are `feature scaling` and `mean normalization`. Feature scaling involves dividing the input values by the range (i.e. the maximum value minus the minimum value) of the input variable, resulting in a new range of just 1. Mean normalization involves subtracting the average value for an input variable from the values for that input variable resulting in a new average value for the input variable of just zero. To implement both of these techniques, adjust your input values as shown in this formula:

<sub></sub>x
<sub>i</sub>
:=
<sub></sub>x
<sub>i</sub> -
<sub></sub>μ
<sub>i</sub>
/ 
<sub></sub>s
<sub>i</sub>

Where 
<sub></sub>μ
<sub>i</sub>
is the `average` of all the values for feature (i) and
<sub></sub>s
<sub>i</sub>
is the range of values (max - min), or
<sub></sub>s
<sub>i</sub>
is the standard deviation.

Note that dividing by the range, or dividing by the standard deviation, give different results. The quizzes in this course use range - the programming exercises use standard deviation.

For example, if
<sub></sub>x
<sub>i</sub>
represents housing prices with a range of 100 to 2000 and a mean value of 1000, then,
<sub></sub>x
<sub>i</sub>
:=
price - 1000 / 1900

## Gradient Descent in Practice II - Learning Rate

`Note:` [5:20 - the x -axis label in the right graph should be <sub></sub>θ rather than No. of iterations ]

`Debugging gradient descent.`Make a plot with *number of iterations* on the x-axis. Now plot the cost function, J<sub></sub>(θ) over the number of iterations of gradient descent. If J<sub></sub>(θ) ever increases, then you probably need to decrease α.

`Automatic convergence test.` Declare convergence if J<sub></sub>(θ) decreases by less than E in one iteration, where E is some small value such as 10^(-3) However in practice it's difficult to choose this threshold value.

<img width="540" alt="Screen Shot 2020-06-03 at 9 34 11 AM" src="https://user-images.githubusercontent.com/55514757/83643738-6825ee00-a57e-11ea-93ad-f639c8bdb378.png">

It has been proven that if learning rate α is sufficiently small, then J<sub></sub>(θ) will decrease on every iteration.

<img width="530" alt="Screen Shot 2020-06-03 at 9 34 22 AM" src="https://user-images.githubusercontent.com/55514757/83643745-69efb180-a57e-11ea-897f-a41540b3eebf.png">

To summarize:

If `α` (alpha) is too small: slow convergence.

If `α` (alpha) is too large: ￼may not decrease on every iteration and thus may not converge.

## Features and Polynomial Regression

We can improve our features and the form of our hypothesis function in a couple different ways.

We can combine multiple features into one. For example, we can `combine`
<sub></sub>x
<sub>1</sub>
and
<sub></sub>x
<sub>2</sub>
into a new feature
<sub></sub>x
<sub>3</sub>
by taking 
<sub></sub>x
<sub>1</sub> *
<sub></sub>x
<sub>2</sub>

#### Polynomial Regression

Our hypothesis function need not be linear (a straight line) if that does not fit the data well.

We can `change the behavior or curve` of our hypothesis function by making it a quadratic, cubic or square root function (or any other form).

For example, if our hypothesis function is 
<sub></sub>h
<sub>θ</sub>
(x) = 
<sub></sub>θ
<sub>0</sub>
+
<sub></sub>θ
<sub>1</sub>
<sub></sub>x
<sub>1</sub>
then we can create additional features based on 
<sub></sub>x
<sub>1</sub>,
to get the quadratic function 

<img width="186" alt="Screen Shot 2020-06-03 at 10 03 15 AM" src="https://user-images.githubusercontent.com/55514757/83646488-b1c40800-a581-11ea-81a6-e5cb3ca730d5.png">

