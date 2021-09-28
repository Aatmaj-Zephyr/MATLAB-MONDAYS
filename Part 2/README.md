# [MATLAB MONDAYS💥- Crash Course part-2](https://dev.to/aatmaj/matlab-mondays-crash-course-part-2-2ol1)

Originally published on the dev.to platform [here](https://dev.to/aatmaj/matlab-mondays-crash-course-part-2-2ol1)

Welcome all! ❤️‍🔥 Let us learn pre-baked MATLAB functions which we can just use off the shelf. After that we will learn the loop in MATLAB.🤟
---
_____
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
> Note that % operator in python is replaced by the mod() function in MATLAB mod(a,b) is equivalent to a%b

_____
That's all for this week. 🏆 Your comments really motivate me, so for any suggestions or doubts, please comments on [dev.to](https://dev.to/aatmaj/matlab-mondays-crash-course-part-2-2ol1), and I will be happy to help 🙂 🎗️ Follow me for updates...

Also, you can gmail me for any suggestion or help 🙌

[![LinkedIn][1.2]][1]
[![Gmail][2.2]][2]


[1.2]: https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white 
[2.2]: https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white

[1]: https://www.linkedin.com/in/aatmajmhatre/
[2]: https://aatmaj.mhatre@gmail.com

