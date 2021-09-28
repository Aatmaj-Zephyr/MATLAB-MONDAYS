# [MATLAB MONDAYS💥- Crash Course part-3](https://dev.to/aatmaj/matlab-mondays-crash-course-part-3-414k)

Originally published on the dev.to platform [here](https://dev.to/aatmaj/matlab-mondays-crash-course-part-3-414k)


Welcome all! ❤️‍🔥 Let us learn about row and column vectors in MATLAB.🤟
---
_____

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

_____
That's all for this week. For any suggestions or doubts, please comment on dev.to [here](https://dev.to/aatmaj/matlab-mondays-crash-course-part-3-414k) or gmail me. 

🎗️ Follow me for updates...


[![LinkedIn][1.2]][1]
[![Gmail][2.2]][2]


[1.2]: https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white 
[2.2]: https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white

[1]: https://www.linkedin.com/in/aatmajmhatre/
[2]: https://aatmaj.mhatre@gmail.com

Bye for now 🖐
Meet you all soon👍

➕➖✖️➗
