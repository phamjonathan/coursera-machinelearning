## Gradient Descent

So we have our hypothesis function and we have a way of measuring how well it fits into the data. Now we need to estimate the parameters in the hypothesis function. That's where gradient descent comes in.

Imagine that we graph our hypothesis function based on its fields
<sub></sub>θ
<sub>0</sub>
and
<sub></sub>θ
<sub>1</sub>
(actually we are graphing the cost function as a function of the parameter estimates). We are not graphing x and y itself, but the parameter range of our hypothesis function and the cost resulting from selecting a particular set of parameters.

We put
<sub></sub>θ
<sub>0</sub>
on the x axis and
<sub></sub>θ
<sub>1</sub>
on the y axis,
with the cost function on the vertical z axis. The points on our graph will be the result of the cost function using our hypothesis with those specific theta parameters. The graph below depicts such a setup.

<img width="580" alt="Screen Shot 2020-06-06 at 10 45 39 AM" src="https://user-images.githubusercontent.com/55514757/83947151-54c78c80-a7e3-11ea-9d1a-f7b8de89d7e8.png">

We will know that we have succeeded when our cost function is at the very bottom of the pits in our graph, i.e. when its value is the minimum. The red arrows show the minimum points in the graph.

The way we do this is by taking the derivative (the tangential line to a function) of our cost function. The slope of the tangent is the derivative at that point and it will give us a direction to move towards. We make steps down the cost function in the direction with the steepest descent. The size of each step is determined by the parameter α, which is called the learning rate.

For example, the distance between each 'star' in the graph above represents a step determined by our parameter α. A smaller α would result in a smaller step and a larger α results in a larger step. The direction in which the step is taken is determined by the partial derivative of
J(
<sub></sub>θ
<sub>0</sub>
<sub></sub>θ
<sub>1</sub>
).
Depending on where one starts on the graph, one could end up at different points. The image above shows us two different starting points that end up in two different places.

<img width="700" alt="Screen Shot 2020-06-06 at 10 47 18 AM" src="https://user-images.githubusercontent.com/55514757/83947161-65780280-a7e3-11ea-94d8-2aed6236a837.png">

<img width="650" alt="Screen Shot 2020-06-06 at 10 47 22 AM" src="https://user-images.githubusercontent.com/55514757/83947193-8fc9c000-a7e3-11ea-8bf7-209aa801feca.png">

## Gradient Descent Intuition

In this video we explored the scenario where we used one parameter
<sub></sub>θ
<sub>1</sub>
and plotted its cost function to implement a gradient descent. Our formula for a single parameter was :

Repeat until convergence:

<img width="168" alt="Screen Shot 2020-06-06 at 10 54 57 AM" src="https://user-images.githubusercontent.com/55514757/83947365-6e1d0880-a7e4-11ea-979b-c627e7c061fc.png">

<img width="610" alt="Screen Shot 2020-06-06 at 10 55 12 AM" src="https://user-images.githubusercontent.com/55514757/83947367-7117f900-a7e4-11ea-8b7d-f639b2b4f54e.png">

On a side note, we should adjust our parameter \alphaα to ensure that the gradient descent algorithm converges in a reasonable time. Failure to converge or too much time to obtain the minimum value imply that our step size is wrong.

<img width="675" alt="Screen Shot 2020-06-06 at 10 57 28 AM" src="https://user-images.githubusercontent.com/55514757/83947411-b805ee80-a7e4-11ea-8922-b24b934e0409.png">

### How does gradient descent converge with a fixed step size α?

<img width="450" alt="Screen Shot 2020-06-06 at 10 59 44 AM" src="https://user-images.githubusercontent.com/55514757/83947451-fb605d00-a7e4-11ea-90c7-718e42965005.png">

<img width="130" alt="Screen Shot 2020-06-06 at 11 00 19 AM" src="https://user-images.githubusercontent.com/55514757/83947452-fdc2b700-a7e4-11ea-8bd9-8088bfdee5a1.png">

<img width="650" alt="Screen Shot 2020-06-06 at 11 01 15 AM" src="https://user-images.githubusercontent.com/55514757/83947480-2cd92880-a7e5-11ea-9241-f0ff4f7509e0.png">

## Gradient Descent For Linear Regression

`Note:` [At 6:15 "h(x) = -900 - 0.1x" should be "h(x) = 900 - 0.1x"]

When specifically applied to the case of linear regression, a new form of the gradient descent equation can be derived. We can substitute our actual cost function and our actual hypothesis function and modify the equation to :

<img width="382" alt="Screen Shot 2020-06-06 at 12 07 31 PM" src="https://user-images.githubusercontent.com/55514757/83948876-695d5200-a7ee-11ea-8b5b-d9e2a227cc3e.png">

where m is the size of the training set,
<sub></sub>θ
<sub>0</sub>
a constant that will be changing simultaneously with
<sub></sub>θ
<sub>1</sub>
and
<sub></sub>x
<sub>i</sub> ,
<sub></sub>y
<sub>i</sub>
are values of the given training set (data).

Note that we have separated out the two cases for
<sub></sub>θ
<sub>j</sub>
into separate equations for 
<sub></sub>θ
<sub>0</sub>
and
<sub></sub>θ
<sub>1</sub> ;
and that for
<sub></sub>θ
<sub>1</sub>
we are multiplying
<sub></sub>x
<sub>i</sub>
at the end due to the derivative.

<img width="410" alt="Screen Shot 2020-06-06 at 12 11 45 PM" src="https://user-images.githubusercontent.com/55514757/83948982-28b20880-a7ef-11ea-8a70-131cd670b286.png">

The point of all this is that if we start with a guess for our hypothesis and then repeatedly apply these gradient descent equations, our hypothesis will become more and more accurate.

So, this is simply gradient descent on the original cost function J. This method looks at every example in the entire training set on every step, and is called `batch gradient descent`. Note that, while gradient descent can be susceptible to local minima in general, the optimization problem we have posed here for linear regression has only one global, and no other local, optima; thus gradient descent always converges (assuming the learning rate α is not too large) to the global minimum. Indeed, J is a convex quadratic function. Here is an example of gradient descent as it is run to minimize a quadratic function.

<img width="315" alt="Screen Shot 2020-06-06 at 12 14 55 PM" src="https://user-images.githubusercontent.com/55514757/83949020-63b43c00-a7ef-11ea-809a-4c5a91e6c700.png">

The ellipses shown above are the contours of a quadratic function. Also shown is the trajectory taken by gradient descent, which was initialized at (48,30). The x’s in the figure (joined by straight lines) mark the successive values of
<sub></sub>θ
that gradient descent went through as it converged to its minimum.

