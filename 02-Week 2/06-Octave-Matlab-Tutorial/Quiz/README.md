## Octave/Matlab Tutorial

#### Question 1:

    A = [1 2; 3 4; 5 6];
    B = [1 2 3; 4 5 6];

Which of the following are then valid commands? Check all that apply. (Hint: A' denotes the transpose of A.)

    C = A' + B;

    C = B * A;

    C = A + B;

    C = B` * A;

`Answer:`


#### Question 2:

    Let x = [ 16  2  3  13 ]
            [ 5  11  10  8 ]
            [ 9  7   6  12 ]
            [ 4  14  15  1 ]

Which of the following expression gives 

    B = [ 16 2 ]
        [ 5 11 ]
        [ 9  7 ]
        [ 4 14 ]

Check that all apply.

    B = A(:, 1:2);

    B = A(1:4, 1:2);

    B = A(0:2, 0:4)

    B = A(1:2, 1:4);

`Answer:`


#### Question 3:

Let A be a 10x10 matrix and x be a 10-element vector. Your friend wants to compute the product Ax and writes the following code:

<img width="315" alt="Screen Shot 2020-06-09 at 7 35 42 PM (2)" src="https://user-images.githubusercontent.com/55514757/84211150-a6447580-aa88-11ea-9801-20fd2750cfef.png">

    v = A * x;

    v = Ax;

    v = x' * A;

    v = sum (A * x);

`Answer:`



#### Question 4:

Say you have two column vectors vv and ww, each with 7 elements (i.e., they have dimensions 7x1). Consider the following code:

<img width="230" alt="Screen Shot 2020-06-09 at 7 39 24 PM (2)" src="https://user-images.githubusercontent.com/55514757/84222481-b1f26500-aaa5-11ea-90b7-5fbc86fa3e7f.png">

Which of the following vectorizations correctly compute z? Check all that apply.

    z = sum (v .* w);

    z = v' * w;

    z = v * w';

    z = v .* w;

`Answer:`



#### Question 5:

In Octave, many functions work on single numbers, vectors, and matrices. For example, the sin function when applied to a matrix will return a new matrix with the sin of each element. But you have to be careful, as certain functions have different behavior. Suppose you have an 7x7 matrix X. You want to compute the log of every element, the square of every element, add 1 to every element, and divide every element by 4. You will store the results in four matrices, A,B,C,D. One way to do so is the following code:

<img width="310" alt="Screen Shot 2020-06-09 at 7 39 33 PM (2)" src="https://user-images.githubusercontent.com/55514757/84222490-b61e8280-aaa5-11ea-8303-ee549fd86b9e.png">

Which of the following correctly compute A,B,C, or D? Check all that apply.

    C = X + 1;

    D = X / 4;

    A = log (X);

    B = X ^ 2;

`Answer:`
