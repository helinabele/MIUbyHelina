# MIUbyHelina
1. Write a function named countDigit that returns the number of times that a given digit appears in a positive
number. For example countDigit(32121, 1) would return 2 because there are two 1s in 32121. Other examples:
          countDigit(33331, 3) returns 4
          countDigit(33331, 6) returns 0
          countDigit(3, 3) returns 1140
The function should return -1 if either argument is negative, so countDigit(-543, 3) returns -1.
The function signature is int countDigit(int n, int digit)
Hint: Use modulo base 10 and integer arithmetic to isolate the digits of the number.
2. A Bunker array is defined to be an array in which at least one odd number is immediately followed by a
prime number. So {4, 9, 6, 7, 3} is a Bunker array because the odd number 7 is immediately followed by the
prime number 3. But {4, 9, 6, 15, 21} is not a Bunker array because none of the odd numbers are immediately
followed by a prime number.
Write a function named isBunkerArray that returns 1 if its array argument is a Bunker array, otherwise it
returns 0.141
If you are programming in Java or C#, the function signature is int isBunkerArray(int [ ] a)
If you are programming in C or C++, the function signature is
int isBunkerArray(int a[ ], int len) where len is the number of elements in the array.
You may assume that there exists a function isPrime that returns 1 if it argument is a prime, otherwise it
returns 0. You do not have to write this function.
3. A Meera array is defined to be an array such that for all values n in the array, the value 2*n is not in the
array. So {3, 5, -2} is a Meera array because 3*2, 5*2 and -2*2 are not in the array. But {8, 3, 4} is not
a Meera array because for n=4, 2*n=8 is in the array.
Write a function named isMeera that returns 1 if its array argument is a Meera array. Otherwise it returns 0.
If you are programming in Java or C#, the function signature is
int isMeera(int [ ] a)
If you are programming in C or C++, the function signature is
int isMeera(int a[ ], int len) where len is the number of elements in the array.
