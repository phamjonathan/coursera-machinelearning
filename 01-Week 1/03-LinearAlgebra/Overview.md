### Matrices and Vectors

Matrices are 2-dimensional arrays:

            [ a b cd e f g h ij k l ]

The above matrix has four rows and three columns, so it is a 4 x 3 matrix.
A vector is a matrix with one column and many rows:

            [ wxyz ]

### Notation and terms:

* Ai jrefers to the element in the ith row and jth column of matrix A.

* A vector with 'n' rows is referred to as an 'n'-dimensional vector.

* Vi refers to the element in the ith row of the vector.

* In general, all our vectors and matrices will be 1-indexed. Note that for some programming languages, the arrays are 0-indexed.

* Matrices are usually denoted by uppercase names while vectors are lowercase.

* "Scalar" means that an object is a single value, not a vector or matrix.

* R refers to the set of scalar real numbers.

* R^n refers to the set of n-dimensional vectors of real numbers.
Run the cell below to get familiar with the commands in Octave/Matlab. Feel free to create matrices and vectors and try out different things.

1. % The ; denotes we are going back to a new row. 

        A = [1, 2, 3; 4, 5, 6; 7, 8, 9; 10, 11, 12] 

2. % Initialize a vector

        V = [1;2;3] 

3. % Get the dimension of the matrix A where m = rows and n = columns

        [m,n] = size(A) 

4. % You could also store it this way

        dim_A = size(A)

5. % Get the dimension of the vector v 

        dim_v = size(v) 

6. % Now let's index into the 2nd row 3rd column of matrix A

        A_23 = A(2,3)


### Results

1.

        A = 

        1    2    3
        4    5    6
        7    8    9
        10   11   12

2.

        V = 
    
        1        
        2        
        3        
         
3.

        m = 4     
        n = 3       

4.

        dim_A =

        4   3        
            
5.

        dim_v =

        3   1   

6.

        A_23 =

        6    

### Addition and Scalar Multiplication

Addition and subtraction are element-wise, so you simply add or subtract each corresponding element:

    [ a bc d ] + [ w xy z ] = [ a + w  b + xc + y  d + z ]    

Subtracting Matrices:

    [ a bc d ] - [ w xy z ] = [ a - w  b - xc - y  d - z ] 

 To add or subtract two matrices, their dimensions must be `the same`.

In scalar multiplication, we simply multiply every element by the scalar value:

In scalar division, we simply divide every element by the scalar value:

    [ a bc d ] / x = [ a/b  b/xc/y  d/x ] 

Experiment below with the Octave/Matlab commands for matrix addition and scalar multiplication. Feel free to try out different commands. Try to write out your answers for each command before running the cell below.

