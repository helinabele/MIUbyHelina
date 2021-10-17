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
7. Write a function called goodSpread that returns 1 if no value in its array argument occurs more than 3
times in the array.
For example, goodSpread(new int[] {2, 1, 2, 5, 2, 1, 5, 9} returns 1 because no value occurs more than three times.139
But goodSpread(new int[ ] {3, 1, 3 ,1, 3, 5, 5, 3} ) returns 0 because the value 3 occurs four times.
If you are writing in Java or C#, the function signature is int goodSpread (int[ ] a)
If you are writing in C or C++, the function signature is int goodSpread (int a[ ], int len) where len is the number of elements in the array.
8. An Evens number is an integer whose digits are all even. For example 2426 is an Evens number but 3224 is not.
Write a function named isEvens that returns 1 if its integer argument is an Evens number otherwise it returns 0.
9. An array is defined to be a Magic array if the sum of the primes in the array is equal to the first element of the array. If there are no primes in the array, the first element must be 0. So {21, 3, 7, 9,11 4, 6} is a Magic array because 3, 7, 11 are the primes in the array and they sum to 21 which is the first element of the array. {13, 4, 4, 4, 4} is also a Magic array because the sum of the primes is 13 which is also the first element. Other Magic arrays are {10, 5, 5}, {0, 6, 8, 20} and {3}. {0} is not a
Magic array because the sum of the primes is 5+5+3 = 13. Note that -5 is not a prime because prime numbers are positive.
Write a function named isMagicArray that returns 1 if its integer array argument is a Magic array. Otherwise it returns 0.
If you are writing in Java or C#, the function signature is int isMagicArray (int[ ] a)
If you are writing in C or C++, the function signature is int isMagicArray (int a[ ], int len) where len is the number of elements in the array.
You may assume that a function named isPrime exists that returns 1 if its int argument is a prime,
otherwise it returns 0. You do not have to write this function! You are allowed to use it.
10. An array is defined to be complete if the conditions (a), (d) and (e) below hold.
          a. The array contains even numbers
          b. Let min be the smallest even number in the array.
          c. Let max be the largest even number in the array.
          d. min does not equal max
          e. All numbers between min and max are in the array
For example {-5, 6, 2, 3, 2, 4, 5, 11, 8, 7} is complete because
          a. The array contains even numbers
          b. 2 is the smallest even number
          c. 8 is the largest even number
          d. 2 does not equal 8
          e. the numbers 3, 4, 5, 6, 7 are in the array.
Examples of arrays that are not complete are:
          {5, 7, 9, 13} condition (a) does not hold, there are no even numbers.
          {2, 2} condition (d) does not hold
          {2, 6, 3, 4} condition (e) does not hold (5 is missing)
Write a function named isComplete that returns 1 if its array argument is a complete array. Otherwise it returns 0.
If you are writing in Java or C#, the function signature is int isComplete (int[ ] a)
If you are writing in C or C++, the function signature is int isComplete (int a[ ], int len) where len is the number of elements in the array.
