# [MATLAB MONDAYS💥- Crash Course part-6](https://dev.to/aatmaj/matlab-mondays-crash-course-part-6-2c3c)

Originally published on the Dev.to patform [here](https://dev.to/aatmaj/matlab-mondays-crash-course-part-6-2c3c)

Welcome all! ❤️‍🔥 This Monday let us learn about Accessing vector elements in MATLAB.🤟
---
_____
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

We can access the last element of thee vector using the "end" keyword.

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
x(rows,columns), where rows is an array of rows while columns is array of columns. Here is are two examples which will make things very clear.
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

_____
That's all for this week. 🏆 Your comments really motivate me, so for any suggestions or doubts, please [comment on dev.to](https://dev.to/aatmaj/matlab-mondays-crash-course-part-6-2c3c) 👇, and I will be happy to help 🙂 🎗️ Follow me for updates...
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
