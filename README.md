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
11. A primeproduct is a positive integer that is the product of exactly two primes greater than 1. For example, 22 is primeproduct since 22 = 2 times 11 and both 2 and 11 are primes greater than 1.
Write a function named isPrimeProduct with an integer parameter that returns 1 if the parameter is a
primeproduct, otherwise it returns 0. Recall that a prime number is a positive integer with no factors other than 1 and itself.
You may assume that there exists a function named isPrime(int m) that returns 1 if its m is a prime number. You do not need to write isPrime. You are allowed to use this function.
The function signature int isPrimeProduct(int n)
12. An array is called balanced if its even numbered elements (a[0], a[2], etc.) are even and its odd numbered elements (a[1], a[3], etc.) are odd.
Write a function named isBalanced that accepts an array of integers and returns 1 if the array is balanced, otherwise it returns 0.
Examples: {2, 3, 6, 7} is balanced since a[0] and a[2] are even, a[1] and a[3] are odd. {6, 7, 2, 3, 12} is balanced since a[0], a[2] and a[4] are even, a[1] and a[3] are odd.
          {7, 15, 2, 3} is not balanced since a[0] is odd.
          {16, 6, 2, 3} is not balanced since a[1] is even.
If you are programming in Java or C#, the function signature is int isBalanced(int[ ] a)
If you are programming in C or C++, the function signature is int isBalanced(int a[ ], int len)
where len is the number of elements in the array
13. An array with an odd number of elements is said to be centered if all elements (except the middle one) are strictly greater than the value of the middle element. Note that only arrays with an odd number of elements have a middle element. Write a function named isCentered that accepts an integer array and returns 1 if it is a centered array, otherwise it returns 0.
Examples: {5, 3, 3, 4, 5} is not a centered array (the middle element 3 is not strictly less than all other elements), {3, 2, 1, 4, 5} is centered (the middle element 1 is strictly less than all other elements), {3, 2, 1, 4, 1} is not centered (the middle element 1 is not strictly less than all other elements), {3, 2, 1, 1, 4, 6} is not centered (no middle element since array has even number of elements), {} is not centered (no middle element), {1} is centered (satisfies the condition vacuously).
If you are programming in Java or C#, the function signature is int isCentered(int[ ] a)
If you are programming in C or C++, the function signature is int isCentered(int a[ ], int len)
where len is the number of elements in the array.
14. Given a positive integer k, another positive integer n is said to have k-small factors if n can be written as a product u*v where u and v are both less than k. For instance, 20 has 10-small factors since both 4 and 5 are less than 10 and 4*5 = 20. (For the same reason, it is also true to say that 20 has 6-small factors, 7-small factors, 8-small factors, etc). However, 22 does not have 10-small factors since the only way to factor 22 is as 22 = 2 * 11, and 11 is not less than 10.
Write a function hasKSmallFactors with signatuare boolean hasKSmallFactors(int k, int n) which returns true if n has k-small factors. The function should return false if either k or n is not positive.
Examples:
          hasKSmallFactors(7, 30) is true (since 5*6 = 30 and 5 < 7, 6 < 7).
          hasKSmallFactors(6, 14) is false (since the only way to factor 14 is 2*7 = 14 and 7 not less than 6)
          hasKSmallFactors(6, 30) is false (since 5*6 = 30, 6 not less than 6; 3 * 10 = 30, 10 not less than 6; 2 * 15 = 30, 15 not less than 6)
15. Write a function fill with signature
int[ ] fill(int[ ] arr, int k, int n)
which does the following: It returns an integer array arr2 of length n whose first k elements are the same as the first k elements of arr, and whose remaining elements consist of repeating blocks of the first k elements. You can assume array arr has at least k elements. The function should return null if either k or n is not positive.
Examples:
          fill({1,2,3,5, 9, 12,-2,-1}, 3, 10) returns {1,2,3,1,2,3,1,2,3,1}.
          fill({4, 2, -3, 12}, 1, 5) returns {4, 4, 4, 4, 4}.
          fill({2, 6, 9, 0, -3}, 0, 4) returns null.
16. An array is said to be hollow if it contains 3 or more zeroes in the middle that are preceded and followed by the same number of non-zero elements. Write a function named isHollow that accepts an integer array and returns 1 if it is a hollow array, otherwise it returns 0 Examples: isHollow({1,2,4,0,0,0,3,4,5}) returns 1. isHollow ({1,2,0,0,0,3,4,5}) returns 0. isHollow ({1,2,4,9, 0,0,0,3,4, 5}) returns 0. isHollow ({1,2, 0,0, 3,4}) returns 0.
If you are programming in Java or C#, the function signature is int isHollow(int[ ] a).
If you are C or C++ programmer int isHollow(int[ ] a, int len)
where len is the number of elements in the array
17.  Write a function named minDistance that returns the smallest distance between two factors of a number. For example, consider 13013 = 1*7*11*13. Its factors are 1, 7, 11, 13 and 13013. minDistance(13013) would return 2 because the smallest distance between any two factors is 2 (13 - 11 = 2). As another example, minDistance (8) would return 1 because the factors of 8 are 1, 2, 4, 8 and the smallest distance between any two factors is 1 (2 – 1 = 1).
The function signature is int minDistance(int n)
18. A wave array is defined to an array which does not contain two even numbers or two odd
numbers in adjacent locations. So {7, 2, 9, 10, 5}, {4, 11, 12, 1, 6}, {1, 0, 5} and {2} are all wave
arrays. But {2, 6, 3, 4} is not a wave array because the even numbers 2 and 6 are adjacent to each
other.
Write a function named isWave that returns 1 if its array argument is a Wave array, otherwise it returns 0. If you are programming in Java or C#, the function signature is
int isWave (int [ ] a) If you are programming in C or C++, the function signature is int isWave (int a[ ], int len) where len is the number of elements in the array
