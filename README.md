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
4. An integer array is said to be evenSpaced, if the difference between the largest value and the smallest value
is an evennumber. Write a function isEvenSpaced(int[] a) that will return 1 if it is evenSpaced and 0 otherwise.
If array has less than two elements, function will return 0. If you are programming in C or C++, the function
signature is:
int isEvenSpaced (int a[ ], int len) where len is the number of elements in the array.
Examples: Array Largest value Smallest value Difference Return value
          {100, 19, 131, 140} 140 19 140 -19 = 121 0
          {200, 1, 151, 160} 200 1 200 -1 = 199 0
          {200, 10, 151, 160} 200 10 200 -10 = 190 1
          {100, 19, -131, -140} 100 -140 100 - (-140 ) = 240 1
          {80, -56, 11, -81} 80 -81 -80 - 80 = -161 0
5. An Sub array is defined to be an array in which each element is greater than sum of all
elements after that. See examples below:
          {13, 6, 3, 2} is a Sub array. Note that 13 > 2 + 3 + 6, 6 > 3 + 2, 3 > 2.
          {11, 5, 3, 2} is a NOT a Sub array. Note that 5 is not greater than 3 + 2.
Write a function named isSub that returns 1 if its array argument is a Sub array, otherwise it returns 0.
If you are programming in Java or C#, the function signature is: int isSub (int [ ] a)
If you are programming in C or C++, the function signature is: int isSub (int a[ ], int len) where len is the number of elements in the array.
6. An isSym (even/odd Symmetric) array is defined to be an array in which even numbers and odd numbers
appear in the same order from “both directions”. You can assume array has at least one element. See
examples below:
          {2, 7, 9, 10, 11, 5, 8} is a isSym array.
Note that from left to right or right to left we have even, odd, odd, even, odd, odd, even.
          {9, 8, 7, 13, 14, 17} is a isSym array.
Note that from left to right or right to left we have {odd, even, odd, odd, even, odd}.
However, {2, 7, 8, 9, 11, 13, 10} is not a isSym array.
          From left to right we have {even, odd, even, odd, odd, odd, even}.
          From right to left we have {even, odd, odd, odd, even, odd, even}, whichis not the same.
Write a function named isSym that returns 1 if its array argument is a isSym array, otherwise it returns 0.
If you are programming in Java or C#, the function signature is: int isSym (int [ ] a)
If you are programming in C or C++, the function signature is: int isSym (int a[ ], int len) where len is the number of elements in the array.
