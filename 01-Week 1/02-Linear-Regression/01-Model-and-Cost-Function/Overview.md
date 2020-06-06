## Model Representation

<img width="455" alt="Screen Shot 2020-06-05 at 11 54 49 AM" src="https://user-images.githubusercontent.com/55514757/83897546-b6282680-a723-11ea-8c4f-0c349735bce7.png">

Note that the superscript “(i)” in the notation is simply an index into the training set, and has nothing to do with exponentiation. We will also use X to denote the space of input values, and Y to denote the space of output values. In this example, X = Y = ℝ.

To describe the supervised learning problem slightly more formally, our goal is, given a training set, to learn a function h : X → Y so that h(x) is a “good” predictor for the corresponding value of y. For historical reasons, this function h is called a hypothesis. Seen pictorially, the process is therefore like this:

<img width="400" alt="Screen Shot 2020-06-05 at 11 58 53 AM" src="https://user-images.githubusercontent.com/55514757/83933727-36c54200-a779-11ea-8047-376f3e084993.png">

When the target variable that we’re trying to predict is continuous, such as in our housing example, we call the learning problem a regression problem. When y can take on only a small number of discrete values (such as if, given the living area, we wanted to predict if a dwelling is a house or an apartment, say), we call it a classification problem.

## Cost Function

We can measure the accuracy of our hypothesis function by using a `cost function`. This takes an average difference (actually a fancier version of an average) of all the results of the hypothesis with inputs from x's and the actual output y's.

<img width="430" alt="Screen Shot 2020-06-05 at 10 12 41 PM" src="https://user-images.githubusercontent.com/55514757/83933803-daaeed80-a779-11ea-8f34-9d419282f36b.png">

<img width="675" alt="Screen Shot 2020-06-05 at 10 12 56 PM" src="https://user-images.githubusercontent.com/55514757/83933815-f6b28f00-a779-11ea-87af-d144da0acf13.png">

## Cost Function - Intuition I

If we try to think of it in visual terms, our training data set is scattered on the x-y plane. We are trying to make a straight line 
( 
defined by
<sub></sub>h
<sub>θ</sub> (x)
)

Our objective is to get the best possible line. The best possible line will be such so that the average squared vertical distances of the scattered points from the line will be the least. Ideally, the line should pass through all the points of our training data set. In such a case, the value of 
J(
<sub></sub>θ
<sub>0</sub>,
<sub></sub>θ
<sub>1</sub>
)
will be 0. The following example shows the ideal situation where we have a cost function of 0.

<img width="440" alt="Screen Shot 2020-06-05 at 11 20 36 PM" src="https://user-images.githubusercontent.com/55514757/83935031-89a3f700-a783-11ea-88a5-65e32975b86b.png">

When
<sub></sub>θ
<sub>1</sub> = 1,
we get a slope of 1 which goes through every single data point in our model. Conversely, when
<sub></sub>θ
<sub>1</sub> = 0.5,
we see the vertical distance from our fit to the data points increase.

<img width="420" alt="Screen Shot 2020-06-05 at 11 20 49 PM" src="https://user-images.githubusercontent.com/55514757/83935048-a2aca800-a783-11ea-891d-963b5d85e87e.png">

This increases our cost function to 0.58. Plotting several other points yields to the following graph:

<img width="310" alt="Screen Shot 2020-06-05 at 11 20 54 PM" src="https://user-images.githubusercontent.com/55514757/83935074-fd460400-a783-11ea-9357-8d24b536821c.png">

Thus as a goal, we should try to minimize the cost function. In this case,
<sub></sub>θ
<sub>1</sub> = 1
is our global minimum.

## Cost Function - Intuition II

A contour plot is a graph that contains many contour lines. A contour line of a two variable function has a constant value at all points of the same line. An example of such a graph is the one to the right below.

<img width="670" alt="Screen Shot 2020-06-05 at 11 27 28 PM" src="https://user-images.githubusercontent.com/55514757/83935143-ac82db00-a784-11ea-9f9a-33d4ceb9d5ee.png">

Taking any color and going along the 'circle', one would expect to get the same value of the cost function. For example, the three green points found on the green line above have the same value for
J(
<sub></sub>θ
<sub>0</sub>,
<sub></sub>θ
<sub>1</sub>
)
and as a result, they are found along the same line. The circled x displays the value of the cost function for the graph on the left when
<sub></sub>θ
<sub>0</sub> = 800
and
<sub></sub>θ
<sub>1</sub> = -0.15.
Taking another h(x) and plotting its contour plot, one gets the following graphs:

<img width="655" alt="Screen Shot 2020-06-05 at 11 27 34 PM" src="https://user-images.githubusercontent.com/55514757/83935146-b60c4300-a784-11ea-8a96-a23cafcbd21d.png">

when
<sub></sub>θ
<sub>0</sub> = 360
and
<sub></sub>θ
<sub>1</sub> = 0,
the value of
J(
<sub></sub>θ
<sub>0</sub>,
<sub></sub>θ
<sub>1</sub>
)
in the contour plot gets closer to the center thus reducing the cost function error. Now giving our hypothesis function a slightly positive slope results in a better fit of the data.

<img width="640" alt="Screen Shot 2020-06-05 at 11 27 42 PM" src="https://user-images.githubusercontent.com/55514757/83935151-bb698d80-a784-11ea-8143-308bb7a16915.png">

The graph above minimizes the cost function as much as possible and consequently, the result of
<sub></sub>θ
<sub>1</sub>
<sub></sub>θ
<sub>0</sub>
tend to be around 0.12 and 250 respectively. Plotting those values on our graph to the right seems to put our point in the center of the inner most `circle`.