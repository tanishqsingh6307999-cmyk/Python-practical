# Programming Using Python - Practical Record


## Student Details
|field | Details |
|:-----| :------|
|Name  |Aman kumar|
|Course|Bsc (hon) computer science|
|Semester| 1 semester |
| Roll no. | 26570008|
|Subject code | DSC -1|
|Subject|Programming using Python|
|College| Ramanujan College,University of Delhi|
|University|University of Delhi|
|Year |2025-26|


##Practical 1: Find the roots of a quadratic equation
Aim: Write a Python program to find the roots of a quadratic equation.
Equation: 
import cmath

a = float(input("Enter value of a: "))
b = float(input("Enter value of b: "))
c = float(input("Enter value of c: "))

if a == 0:
    print("Not a quadratic equation")
else:
    d = b*b - 4*a*c

    root1 = (-b + cmath.sqrt(d)) / (2*a)
    root2 = (-b - cmath.sqrt(d)) / (2*a)

    print("First root:", root1)
    print("Second root:", root2) 

##Practical 2:
  
