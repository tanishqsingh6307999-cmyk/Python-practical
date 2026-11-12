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

##Practical 2:Wright a program to accept a number 'n'and 
 a. check if 'n'is prime
 b. generate all prime number till 'n'
 c. generate first 'n' prime numbers
this program may be done using functions

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




##Practical 3:Create a pyramid and reverse pyramid using*


n = int(input("Enter number of rows: "))

print("Pyramid:")

for i in range(1, n + 1):
    print(" " * (n - i) + "* " * i)


print("Reverse Pyramid:")

for i in range(n, 0, -1):
    print(" " * (n - i) + "* " * i)

 
 
 ##Practical 4:wright a program that accepts a character  and performs the following:

  a. print whether the character is a letter or numeric digit or a special character. 
  b. if the character is a letter, print whether the letter is uppercase or lowercase. 
  c. if the character is a numeric digit, prints its name in text(e.g, if input is 9,output is NINE) 

s = input("Enter a string: ")

 a. Frequency of a character
ch = input("Enter character to find frequency: ")
print("Frequency:", s.count(ch))


 b. Replace a character
old = input("Enter character to replace: ")
new = input("Enter new character: ")

print("After replacement:", s.replace(old, new))


 c. Remove first occurrence
ch = input("Enter character to remove first occurrence: ")

print("After removing first occurrence:",
      s.replace(ch, "", 1))


 d. Remove all occurrences
ch = input("Enter character to remove completely: ")

print("After removing all occurrences:",
      s.replace(ch, ""))




##Practical 5:Write a program to perform the following operations on a string 

  a. find the frequency of a character in a strig . 
  b. Replace a characters by another  character in a string. 
  c. Remove the first occurrence of acharacter from a string. 
  d. Remove all occurrences of a character from a string. 


s = input("Enter a string: ")

 a. Frequency of a character
ch = input("Enter character to find frequency: ")
print("Frequency:", s.count(ch))


 b. Replace a character
old = input("Enter character to replace: ")
new = input("Enter new character: ")

print("After replacement:", s.replace(old, new))


 c. Remove first occurrence
ch = input("Enter character to remove first occurrence: ")

print("After removing first occurrence:",
      s.replace(ch, "", 1))


 d. Remove all occurrences
ch = input("Enter character to remove completely: ")

print("After removing all occurrences:",
      s.replace(ch, ""))


##Practical 6:Write a program to swap the first n characters of two strings. 

s1 = input("Enter first string: ")
s2 = input("Enter second string: ")

n = int(input("Enter number of characters to swap: "))

if n < 0 or n > len(s1) or n > len(s2):
    print("Invalid number of characters")

else:
    new_s1 = s2[:n] + s1[n:]
    new_s2 = s1[:n] + s2[n:]

    print("First string after swapping:", new_s1)
    print("Second string after swapping:", new_s2)




##Practical 7:








def find_occurrences(str1, str2):

    indices = []
    start = 0

    while True:
        index = str1.find(str2, start)

        if index == -1:
            break

        indices.append(index)
        start = index + 1

    if len(indices) == 0:
        return -1

    return indices


s1 = input("Enter first string: ")
s2 = input("Enter second string: ")

result = find_occurrences(s1, s2)

print("Result:", result)


