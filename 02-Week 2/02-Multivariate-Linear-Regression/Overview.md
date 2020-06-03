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

