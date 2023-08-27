# Missing numbers in array of natural numbers

[Problem link](https://practice.geeksforgeeks.org/problems/missing-number-in-array1416/1)

My Approach:

1. **Initial straithforward approach with two loops**

    Time Complexity: O(n)

    Create an array which includes all the numbers from 1 to (N-1). Run two loops over both the arrays comparing each element of the natural numbers array with each element of the input array. The number which is not found after looping should be returned as the missing element.

2. **Using Hashmap**

    Time complexity: O(n)
    Space complexity: O(n)

    Put all values from the input array in a hashmap. Run a loop from 1 to (N-1) and look for each value in the hashmap. The number which is not found should be returned as the missing element.

Solution:

1. Using Hashing

    Create a temporary array of all zeros. Loop through the input array and set the corresponding element in the temporary array to 1. Loop over the array. The index of the element which is 0 in the temporary array is the missing number.  

2. Using [[Sum of first N natural numbers]]

    Time complexity: O(n)
    Space complexity: O(1)

    Sum of N natural number - Sum of input array = Missing number

    **Drawback**: If the number N is large, it can cause, integer overflow.

    **Workaround for this**: Instead of adding and creating a huge sum which can overflow, add a counter from 1 to (N-1) to the sum (Sum of natural numbers), but subtract the corresponding element of the input array from the sum side by side. The resultant at the end will be the number which is missing. Since it will be added via your counter, but won't be subtracted via the input array.

