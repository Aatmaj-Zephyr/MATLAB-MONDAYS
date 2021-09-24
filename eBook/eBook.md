<p align=center><img src="https://user-images.githubusercontent.com/83284294/134473703-d9ae9e5c-66b5-4b85-a550-de31ce00bbcb.jpg"></img></p>

# MATLAB CRASH COURSE
## A quickstart guide to master MATLAB basics
### _by Aatmaj-Zephyr_

<div style="page-break-after: always;"></div>

# MATLAB CRASH COURSE

### _Forward_
This book covers all essential basics of MATLAB along with relevant code examples. This book is a quickstart guide towards learning MATLAB and not a comprehensive reference encyclopedia. This book focuses more on speed and pace rather than technical completeness.

MATLAB is very easiy to learn language. Using this book, you can master MATLAB in at most three hours. This book is designed in such a manner that it will give you a very clear idea of what MATLAB is and help you cover most of the basics in a very short span of time.

 Before you proceed to learn MATLAB, however I would like to share a few words of caution.MATLAB is neither free nor open. Unless you are a student affiliated to any university 
 MATLAB might not be the best fit for you. However, there are good alternatives to MATLAB. Among them options, I would  advise two alternatives- Python (with scientific add-ons) and the Julia language. Julia is a better alternative to MATLAB with syntax very similar to it. However one point of advantage of learning MATLAB is that the syntax of MATLAB is very similar to that of GNU Octave, a free alternative to MATLAB. 
 
 I hope that you will find the contents of this book at your advantage.
 
____
**Prerequisites-** Basic knowledge of programming. (Variables, Control statements, etc)

<div style="page-break-after: always;"></div>

## Chapter One: Introduction

**What is MATLAB?**- MATLAB stands for MATrix LABoratory. MATLAB is a scientific programming language.✨ It is mainly used for solving mathematical equations and data-visualization. Complicated systems can be better understood with this software. Speed and ease of writing are the salient features of MATLAB.
Professor Cleve Moler designed MATLAB. He did so with an intention to reduce heavy FORTRAN coding. The aim of the language was making an engineer friendly syntax.

<p align=center><img src="https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ccd2tfo3drskbka1svmi.png"></img></p>


MATLAB is used by students and engineers in many disciplines like Robotics, Astrology, Machine Learning, Image Processing and Biology. 

**MATLAB web browser** The MATLAB web browser let's us run MATLAB through the web. First, login (create a new account) using your university account. If you do not have a university account, you can use a free 30- day trial too!

<p align=center><img src="https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1cc7d7t2q2synxnwuutp.png"></img></p>

**The command prompt**
MATLAB online contains the command prompt central to the page, where we can write our code. Similar to python, MATLAB let's us calculate numbers at the command prompt, and the answer is displayed in the command window. 

![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/40fipam8fjgg66h1eiy4.png)

Adding a semicolon at the end of the statement prevents output from being displayed.

![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/6tqukdai7gi74n6s1auz.png)

Similer to many languages, too small or too large values like the last one are displayed using scientific notation.

 MATLAB operators follow this order-
> 1) Parenthesis
> 2) Exponentiation
> 3) Product and Division
> 4) Addition and Subtraction

So for complicated calculations, it is important to specify the brackets.

The command prompt can be quit using the command "exit"
 
**MATLAB VARIABLES**
We can declare variables using the '=' sign, that is the assignment operator.
The following are the rules for variable declaration in MATLAB are same as Python as below
> Variables must begin with a letter, are case sensitive, may contain only letters numbers or underscores

The variables declared are located at the left bottom side of the page. (WORKSPACE) The values of the variables are also displayed along with their class. Note that MATLAB treats 'ans' as a variable too. So whenever operations are performed, the variable 'ans' is overridden.

![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/2jgrt0mzigicavtbg2il.png)

<div style="page-break-after: always;"></div>

## Chapter Two: Inbuilt Functions and Control Statements

**In built Functions in MATLAB**

MATLAB supports standered mathematical functions like sin, cos, log, exponentiation, square root, and many more.
However, unlike many languages, input for these functions can be an integer or even an matrix vectors.
Many MATLAB functions take in multiple inputs and return multiple outputs. eg. the min function can take in an array of numbers and output both, the smallest number and the position of the smallest number.

![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8ppw8z00p8mjxwob6hnd.png)

Similarly, the function plot takes in two matrices and plots their values. The plot connects all the points represented by the x,y pairs.
![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/57t4pvhadx7ad0lciz82.png)
 
 
Another similer function is scatter() which generates the scatterplot of the functions.
![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/i44d8kzajd7xo0jf9s89.png)
 MATLAB contains loads of other functions, whose documentation can be found out [here](https://in.mathworks.com/help/matlab/elementary-math.html?s_tid=CRUX_lftnav)

One more valuable function is rand(), which returns a random value.
```
>> x=rand()

x =

    0.8147
```
____
**Program control statements**
MATLAB has the for loop syntax as follows
```MATLAB
for i=a:b
 c=d
end
```
Here the running variable i assumes values from 0,99
Python equivalent of this statement is 
```python
for i in range(a,b):
 #function
```

Here is a sample program-

![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hrcivocu7cnwsmjzonzk.png)
 
The if else statement has the following syntax
```MATLAB
if a<b
 a=b
elseif a>b
 a=0
else
 b=0
end
```
The Python equivalent is 
```python
if a<b:
 a=b
elif a>b:
 a=0
else:
 b=0
```

Here is a sample 
```MATLAB
>> x=10;
>> if x<10
x=3
>> elseif x==10
>> x=pi
>> else
>> x=100
>> end
x =

    3.1416
```

**While loop**
 MATLAB also has the while loop with syntax as
```MATLAB
while condition
statement
end
```
For an infinite loop, 

```MATLAB
while true
 statement
end
```

Here is an example which uses while loop- the Collatz conjuncture

```MATLAB
>> for k=1:100
x=k;
while x>1
if mod(x,2)==0
x=x/2
else
x=3*x+1
end
end
end
```
> Note that % operator in python is replaced by the mod() function in MATLAB. mod(a,b) is equivalent to a%b

<div style="page-break-after: always;"></div>

## Chapter Three: Row and Column Vectors

**Row and Column Vectors in MATLAB**
We can create row vector in matlab by this syntax-
```MATLAB
x=[-2,-1,0,-1,-2]
```
Similarly we can make column vectors using ':' instead of ','
```MATLAB
x=[-2;-1;0;-1;-2]
```
Here is the output-
```MATLAB
>> x=[2;3;4;5];
>> x

x =

     2
     3
     4
     5

>> x=[2,3,4,5,];
>> x

x =

     2     3     4     5
```
 
Sometimes, however we may require to create row or column vectors with large number of equidistant points. Example, for plotting values from -2 to 2, we may require to plot at steps of small units like 0.01. In that case, MATLAB provides a feature to unable creation of "Uniformly Based Vectors" 
We can create such vectors by inputting startvalue, spacing and end value -
```MATLAB
x=startvalue: spacing: endvalue
```
Here is an example-
```MATLAB
>> x=-1:0.17:+1

x =

   -1.0000   -0.8300   -0.6600   -0.4900   -0.3200   -0.1500    0.0200    0.1900    0.3600    0.5300    0.7000    0.8700

```
 
 
> Note- Vector ends on the largest value within  range. That is, after adding up consecutive spacing values, vector ends in the greatest value smaller than the endvalue

If the spacing value is not mentioned, it defaults to one-
```MATLAB
>> y=[-4:5]

y =

    -4    -3    -2    -1     0     1     2     3     4     5

```
Similarly, all this can be done for column vectors as well



**The transpose operator**
The row vectors can be transformed into column vectors using the transpose operator 
```MATLAB
x=(Startvalue:spacing:endvalue)'
```
This operator transposes any matrix (flips over rows and columns)
```MATLAB
>> z=(-3:1)

z =

    -3    -2    -1     0     1

>> x=(z)'

x =

    -3
    -2
    -1
     0
     1
```

<div style="page-break-after: always;"></div>

## Chapter Four: Matrices in MATLAB

**Making matrices in MATLAB**
We will now learn how to create Matrices in MATLAB.
Similer to row vectors, the elements in a row are separated by a ',' and column by a ';'. First, type in the values for the first column separated by commas. When the row ends, type a semicolon and the proceed on to the next row. Repeat until done, and end with the square brackets.

![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/6tr3x2ne4hn7pqq72coj.png)

Mismatch of elements in rows or columns generates this error-

![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/aa6dzbd8321mh79qhlia.png)
 
**Fusing two Matrices**
In a similar way of making matrices, we can combine them together with this syntax
```Matlab
a=[  ]
b=[  ]
c=[a;b]
```
This is vertical concatenation. The two matrices will be placed one on top of the other and joined together

For horizontal concatenation, use the syntax c=[a,b]

![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/0l0pjrk9v054nmo2v6rw.png)

> Note, For horizontal Concatenation, the number of rows for both matrices must be the same, and for vertical concatenation, the number of columns must be equal. If tis rule is violated, Concatenation error is generated. 

**Matrix generation functions**
There are a few matrix generation functions in MATLAB like eye() this function generates an Identity matrix of the size we input.
example-
```MATLAB
>> I=eye(10)

I =

     1     0     0     0     0     0     0     0     0     0
     0     1     0     0     0     0     0     0     0     0
     0     0     1     0     0     0     0     0     0     0
     0     0     0     1     0     0     0     0     0     0
     0     0     0     0     1     0     0     0     0     0
     0     0     0     0     0     1     0     0     0     0
     0     0     0     0     0     0     1     0     0     0
     0     0     0     0     0     0     0     1     0     0
     0     0     0     0     0     0     0     0     1     0
     0     0     0     0     0     0     0     0     0     1
```
 The zeros() function creates a square martix of zeros
For rectangular matrices, two arguments can be used.
```MATLAB
>> z=zeros(3)

z =

     0     0     0
     0     0     0
     0     0     0

>> z=zeros(3,5)

z =

     0     0     0     0     0
     0     0     0     0     0
     0     0     0     0     0
```
We can use the exact same syntax for the ones function and the rand function.

```MATLAB
>> x=rand(5,6)

x =

    0.8147    0.0975    0.1576    0.1419    0.6557    0.7577
    0.9058    0.2785    0.9706    0.4218    0.0357    0.7431
    0.1270    0.5469    0.9572    0.9157    0.8491    0.3922
    0.9134    0.9575    0.4854    0.7922    0.9340    0.6555
    0.6324    0.9649    0.8003    0.9595    0.6787    0.1712

>> x=ones(5,6)

x =

     1     1     1     1     1     1
     1     1     1     1     1     1
     1     1     1     1     1     1
     1     1     1     1     1     1
     1     1     1     1     1     1
```

Similarly there is the diag function for a diagonal matrix
```MATLAB
>> x=diag(1:7)

x =

     1     0     0     0     0     0     0
     0     2     0     0     0     0     0
     0     0     3     0     0     0     0
     0     0     0     4     0     0     0
     0     0     0     0     5     0     0
     0     0     0     0     0     6     0
     0     0     0     0     0     0     7
```

<div style="page-break-after: always;"></div>

## Chapter Five: Calculations on Matrices

**Matrix calculations**
We may at times require to manipulate the individual elements of matrices. We can make these matrix calculations similar to variable operations.
Example we want to make a matrix y such that each element in y is twice that of each in x. We can do so by y=2*x

```MATLAB
>> x=[1,2,3,4,5];
>> y=2*x

y =

     2     4     6     8    10
```

Now, if we want to make another vector z which is the addition  in x and y, z=x+y
```MATLAB
>> z=x+y

z =

     3     6     9    12    15

>> z=x-y

z =

    -1    -2    -3    -4    -5
```
However, when we multiply the two, an error occurs.
![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/yxg91fqmrc1y8dy3tblo.png)
This is because the 8 operator means matrix multiplication and not element wise multiplication. For element wise multiplication, we use ".*". Similar for division "./" and exponentiation ".^"

```MATLAB
>> z=y.*x

z =

     2     8    18    32    50

>> z=x./y

z =

    0.5000    0.5000    0.5000    0.5000    0.5000

>> z=x.^y

z =

           1          16         729       65536     9765625

```

> When dealing with two matrices, always add a dot before operators for making "element wise operators "-.*" , "./" and ".^". This is because normal operators are reserved for matrix operations.

Note, the matrix operations are only valid for matrices of same sizes and dimensions. If this is not followed, this error pops up-
![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8gsr3uziiwsdoxvc6617.png)

Here is an example of the application of what we learnt so far-
![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/oh4f3ru6vxrkugra8vmu.png)
 Try plotting a few equations yourself....


**Matrix multiplication**
Matrix multiplication can be done easily by just multiplying the two together. However, be careful that the dimensions for  matrix multiplication match.

```MATLAB
>> x=[1,2,3;4,5,6]

x =

     1     2     3
     4     5     6

>> y=[1,2;3,4;5,6]

y =

     1     2
     3     4
     5     6

>> x*y

ans =

    22    28
    49    64
```


____

**Statistical functions**
Many times we need to find mean, mode or median of a vector. Such a statistical analysis of the data can be done easily in MATLAB using inbuilt functions.
The mean() function can find the mean of the vector elements, while median() returns the central number.
The mode() gives out the mode of the vector, while var() and std() return the variance and the standered deviations respectively. rms() indicated the root mean square.
Apart from these widely used functions, you will find many more in the MATLAB documentation. 

```MATLAB
>> x=[1,2,3,4,5,4,3,2,1,1];
>> mean(x)

ans =

    2.6000

>> mode(x)

ans =

     1

>> var(x)

ans =

    2.0444

>> std(x)

ans =

    1.4298

>> median(x)

ans =

    2.5000

>> y=median(x).*x

y =

    2.5000    5.0000    7.5000   10.0000   12.5000   10.0000    7.5000    5.0000    2.5000    2.5000

>> rms(x)

ans =

    2.9326
```
<div style="page-break-after: always;"></div>

## Chapter Six Acessing Vector Elements

Many times, we need to access the elements in middle of a vector or matrix. MATLAB provides easy methods to extract out the elements.


**Accessing vector elements**-

We can access and the vector elements as shown in the example
```MATLAB
>> x=[1,2,3,4,0,6];
>> x(5)

ans =

     0

>> x(5)=5;
>> x

x =

     1     2     3     4     5     6
```

MATLAB also allows us to access many elements at once. The result is a 'n' element vector
```MATLAB
>> x=[2,4,6,8];
>> y=x([2,3])

y =

     4     6
>> y=x([1,3,4])

y =

     2     6     8
```
An alternative may be 
```MATLAB
>> x=[2,4,6,8];
>> data=1:3;
>> y=x(data)

y =

     2     4     6
```

We can acess the last element of thee vector using the "end" keyword.

```MATLAB
>> x=[2,4,6,8];
>> x(end)

ans =

     8

>> x(end-1)

ans =

     6
```

**Accessing matrix values**-
Matrix values require both the row and the column number to be accessed
```MATLAB
>> x=rand(5,6)

x =

    0.9058    0.2785    0.9706    0.4218    0.0357    0.7431
    0.1270    0.5469    0.9572    0.9157    0.8491    0.3922
    0.9134    0.9575    0.4854    0.7922    0.9340    0.6555
    0.6324    0.9649    0.8003    0.9595    0.6787    0.1712
    0.0975    0.1576    0.1419    0.6557    0.7577    0.7060

>> x(2,3)

ans =

    0.9572
```

We can also extract a whole matrix using the syntax
x(rows,columns), where rows is a array of rows while columns is array of columns. Here is are two examples which will make things very clear.
![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/m8g4lgx1u1uhkgzekiok.png)

Note that 2:4 means [2,3,4] while comma separated 2,4 means [2,4]
![image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/566x0w1q2fhks3yjeljr.png)
 
 In order to take an entire column or row, we can just place a semicolon ':' for it. Here is an example-
```MATLAB
>> x=rand(5,5)

x =

    0.8314    0.4168    0.0155    0.1981    0.0527
    0.8034    0.6569    0.9841    0.4897    0.7379
    0.0605    0.6280    0.1672    0.3395    0.2691
    0.3993    0.2920    0.1062    0.9516    0.4228
    0.5269    0.4317    0.3724    0.9203    0.5479

>> x(:,3)

ans =

    0.0155
    0.9841
    0.1672
    0.1062
    0.3724

>> x(3,:)

ans =

    0.0605    0.6280    0.1672    0.3395    0.2691
```

<div style="page-break-after: always;"></div>

## Summary of the Book

- **Chapter One** : We had an introduction to what MATLAB is and where is it used. MATLAB stands for MATrix LABoratory. MATLAB is a scientific programming language used for simulations and data driven research. We also wrote our hello world code in this part. After that, we learnt about MATLAB variables. We can declare variables using the '=' sign, that is the assignment operator.
- **Chapter Two**: We learnt about some predefined functions in MATLAB like `rand()` `scatter()` and `min()`. MATLAB contains loads of other functions, whose documentation can be found out on https://in.mathworks.com/help/matlab/elementary-math.html?s_tid=CRUX_lftnav. After that we learnt control statements in MATLAB including the syntax for the while loop, for loop and if-else-elseif statements.
- **Chapter Three**: We studied  row and column vectors in MATLAB. Sometimes, however we may require to create row or column vectors with large number of equidistant points. We learnt how to do that automatically in MATLAB. At the end we also learnt how to take the transpose of any matrix.
- **Chapter Four**: We understood the syntax for the generation of matrices. In a similar way of making matrices, we can combine them together and fuse two matrices. Besides, there also exist inbuilt functions for matrix generation, which we covered in the part.
- **Chapter Five**: We checked out how to operate on matrices in MATLAB. Then we had a look at matrix multiplications Matrix multiplication can be done easily by just multiplying the two together. Many times we need to find mean, mode or median of a vector. Such a statistical analysis of the data can be done easily in MATLAB using inbuilt functions.
- **Chapter Six**: This part was reserved for accessing vectors and matrices. Many times, we need to access the elements in middle of a vector or matrix. MATLAB provides easy methods to extract out the elements. Similarly we can easily access matrices.
