# [MATLAB MONDAYS💥- Crash Course part-5](https://dev.to/aatmaj/matlab-mondays-crash-course-part-5-pm6)

Originally published on the dev.to platform [here](https://dev.to/aatmaj/matlab-mondays-crash-course-part-5-pm6)

Welcome all! ❤️‍🔥 This Monday let us learn about statistical functions and how to calculate on matrices.🤟
---
_____
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
This is because the 8 operator means matrix multiplication and not element wise multiplication. For element wise multiplication, we use `.*`. Similar for division `./` and exponentiation `.^`

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

_____
That's all for this week. 🏆 Your comments really motivate me, so for any suggestions or doubts, please comment below 👇, and I will be happy to help 🙂 🎗️ Follow me for updates...
Also, you can gmail me for any suggestion or help 🙌
[![LinkedIn][1.2]][1]
[![Gmail][2.2]][2]


[1.2]: https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white 
[2.2]: https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white

[1]: https://www.linkedin.com/in/aatmajmhatre/
[2]: https://aatmaj.mhatre@gmail.com

Bye for now 🖐
Meet you all soon👍

➕➖✖️➗
