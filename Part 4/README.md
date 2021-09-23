# MATLAB MONDAYS💥- Crash Course part-4


Originallly published on the dev.to platform [here](https://dev.to/aatmaj/matlab-mondays-crash-course-part-4-2c43)

Welcome all! ❤️‍🔥 This Monday let us learn all about matrices in MATLAB, and how to generate them🤟
---
_____
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

_____
That's all for today. For any suggestions or doubts, please comment on the dev.to platform [here](https://dev.to/aatmaj/matlab-mondays-crash-course-part-4-2c43) (they do motivate me a lot...) 🎗️ Follow me for updates...
Also, you can gmail me for any suggestion or help 🙌 
[![LinkedIn][1.2]][1]
[![Gmail][2.2]][2]


[1.2]: https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white 
[2.2]: https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white

[1]: https://www.linkedin.com/in/aatmajmhatre/
[2]: https://aatmaj.mhatre@gmail.com

Bye for now 🖐
Happy to help always.....😃
Meet you all soon👍

➕➖✖️➗
