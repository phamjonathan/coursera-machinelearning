#### Question 1:

Consider the problem of predicting how well a student does in her second year of college/university, given Consider the problem of predicting how well a student does in her second year of college/university, given how well she did in her first year.

Specifically, let x be equal to the number of "A" grades (including A-. A and A+ grades) that a student receives in their first year of college (freshmen year). We would like to predict the value of y, which we define as the number of "A" grades they get in their second year (sophomore year).

Here each row is one training example. Recall that in linear regression, our hypothesis is h<sub>θ</sub>(x)=θ<sub>0</sub>+θ<sub>1</sub>x, and we use m to denote the number of training examples.

x | y
--- | ---
5 | 4
3 | 4
0 | 1
4 | 3

For the training set given above (note that this training set may also be referenced in other questions in this quiz), what is the value of m? In the box below, please enter your answer (which should be a number between 0 and 10).

Answer: 4

#### Question 2:

For this question, assume that we are using the training set from Q1. Recall our definition of the cost function was 
<sub></sub>J(θ
<sub>0,</sub>θ
<sub>1</sub>)=

Answer: 0.5

#### Question 3:

Suppose we set 
<sub></sub>θ 
<sub>0</sub>=-1,
<sub></sub>θ
<sub>1</sub>=0.5 What is
<sub></sub>H
<sub>θ</sub>(4)?

Answer: 1

#### Question 4:

Let F be some function so that 
<sub></sub>F(θ
<sub>1,</sub>θ
<sub>1</sub>) 
outputs a number. For this problem, F is some arbitrary/unknown smooth function (not necessarily the cost function of linear regression, so F may have local optima). Suppose we use gradient descent to try to minimize 
<sub></sub>F(θ
<sub>1,</sub>θ
<sub>1</sub>) as a function of 
<sub></sub>θ 
<sub>0 and </sub>θ 
<sub>1</sub>
Which of the following statements are true? 

* Even if the learning rate α is very large, every iteration of gradient descent will decrease the value of
<sub></sub>F(θ
<sub>0,</sub>θ
<sub>1</sub>)

* If the learning rate is too small, then gradient descent may take a very long time to converge.

* If 
<sub></sub>θ
<sub>0</sub> and θ
<sub>1</sub>
are initialized at a local minimum, then one iteration will not change their values.

* If
<sub></sub>θ
<sub>0</sub> and θ
<sub>1</sub>
are initialized so that 
<sub></sub>θ
<sub>0</sub> = θ
<sub>1</sub>
then by symmetry (because we do simultaneous updates to the two parameters), after one interation of gradient descent, we still have 
<sub></sub>θ
<sub>0</sub> = θ
<sub>1</sub>

Answers:
* TRUE - If the learning rate is small, gradient descent ends up taking an extremely small step on each iteration, and therefor can take a long time to converge

* TRUE - At a local minimum, the derivative (gradient) is zero, so gradient descent will not change the parameters.

* FALSE - If the learning rate is too large, one step of gradient descent can actually vastly "overshoot" and actually increase the value of 
<sub></sub>F(θ
<sub>1,</sub>θ
<sub>1</sub>)

* FALSE - The updates to 
<sub></sub>θ
<sub>0</sub> and θ 
<sub>1</sub>
are different (even though we're doing simulaneous updates), so there's no particular reason to update them to be same after on interation of gradient descent.

#### Question 5:

Suppose that for some linear regression problem (say, predicting housing prices as in the lecture), we have some training set, and for our training set we managed to find some
<sub></sub>θ
<sub>0</sub>,
<sub></sub>θ
<sub>1</sub>
such that 
<sub></sub>J(θ
<sub>0,</sub>θ
<sub>1</sub>)=0
Which of the statements below must then be true?

* We can perfectly predict the value of y even for new examples that we have not yet seen. (e.g., we can perfectly predict prices of even new houses that we have not yet seen.)

* For these values of
<sub></sub>θ
<sub>0</sub> and 
<sub></sub>θ
<sub>1</sub>
that satisfy 
<sub></sub>J(θ
<sub>0,</sub>θ
<sub>1</sub>) = 0,
we have 
that 
<sub></sub>H
<sub>θ</sub>(x^i) = y^i
<sub>1</sub>)
for every training example (X^i, Y^i)

* We can perfectly predict the value of y even for new examples that we have not yet seen. (e.g., we can perfectly predict prices of even new houses that we have not yet seen.)

* 	Our training set can be fit perfectly by a straight line, i.e., all of our training examples lie perfectly on some straight line.

Answers:
* FALSE 
* TRUE
* FALSE
* TRUE
