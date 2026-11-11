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


Practical 1: Find the roots of a quadratic equation
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




def is_prime(n):
    if n < 2:
        return False

    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False

    return True


n = int(input("Enter a number: "))

# a. Check prime number
if is_prime(n):
    print(n, "is a prime number")
else:
    print(n, "is not a prime number")


# b. Generate prime numbers till n
print("Prime numbers till", n, ":")

for i in range(2, n + 1):
    if is_prime(i):
        print(i, end=" ")

print()


# c. Generate first n prime numbers
print("First", n, "prime numbers:")

count = 0
num = 2

while count < n:
    if is_prime(num):
        print(num, end=" ")
        count += 1

    num += 1

def is_prime(n):
    if n < 2:
        return False

    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False

    return True


n = int(input("Enter a number: "))

# a. Check prime number
if is_prime(n):
    print(n, "is a prime number")
else:
    print(n, "is not a prime number")


# b. Generate prime numbers till n
print("Prime numbers till", n, ":")

for i in range(2, n + 1):
    if is_prime(i):
        print(i, end=" ")

print()


# c. Generate first n prime numbers
print("First", n, "prime numbers:")

count = 0
num = 2

while count < n:
    if is_prime(num):
        print(num, end=" ")
        count += 1

    num += 1


def is_prime(n):
    if n < 2:
        return False

    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False

    return True


n = int(input("Enter a number: "))

# a. Check prime number
if is_prime(n):
    print(n, "is a prime number")
else:
    print(n, "is not a prime number")


# b. Generate prime numbers till n
print("Prime numbers till", n, ":")

for i in range(2, n + 1):
    if is_prime(i):
        print(i, end=" ")

print()


# c. Generate first n prime numbers
print("First", n, "prime numbers:")

count = 0
num = 2

while count < n:
    if is_prime(num):
        print(num, end=" ")
        count += 1

    num += 1

  
