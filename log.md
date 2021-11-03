# 100 Days Of Code - Log
### Day 1: October 27, Wednesday

**Today's Progress**: Started with **arrays** in **Data Structures and Algorithms**.\
                     Also, learned **C++ STL-vectors, maps and sets** since most of the problems I encountered required vectors.
                                          
**Link(s) to work**
1. [Sort an array of 0,1 and 2](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day1_a.cpp)
2. [Remove duplicates from a sorted array](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day1_b.cpp)

[post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_100daysofcode-datastructures-algorithms-activity-6859162020344938496-JuSb)\
[post on Twitter](https://twitter.com/pundhir_rakhi/status/1453401934082183174)

### Day 2: October 28, Thursday

**Today's Progress**: Problem Statement : [Given two sorted arrays, merge them into one sorted array in constant space](https://leetcode.com/problems/merge-sorted-array/)
                      At first, I couldn't find a method to solve this in O(1) space but later resolved it and realized that whenever we need to solve a task in *constant space* or *optimal time* we can make use of pointers.here, we are taking **three pointers** one at end of first array, the other at end of second array and the third one at the end of total size of first array.Then we start comparing values pointed by the first two pointers and the greater one is placed at the position pointed by the third pointer.At last we come to the beginning of the array which is sorted.
                                                              
**Link(s) to work**
1. [Merge two sorted arrays](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day2.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1453776797544292374)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day2-100daysofcode-100daysofcoding-activity-6859540895470108672-uzmq)

### Day 3: October 29, Friday

**Today's Progress**: Problem : **Maximum Subarray Sum**
             Since the array can have negative values the answer will not be the sum of entire array values.The Brute force is to use nested for loops to compare for each subarray then return the maximum sum.This method has a Time Complexity of O(n2).
             I figured out how simple and optimal(O(n)) is to solve this problem using Kadane's Algorithm. Here, we have to maintain two values, one that contains the current sum obtained so far while traversing the array and the other one to store the maximum of the current sum obtained.If at any point the current sum becomes negative, it is initialized to zero.Finally we return the maximum sum. How this algorithm brings down the Time Complexity is quite appreciating.
             
**Link(s) to work**
1. [Maximum Subarray Sum](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day3.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1454141348043317252)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day3-100daysofcode-arrays-activity-6859904690054922240-6hHp)

### Day 4: October 30, Saturday

**Today's Progress**: Problems: 1. [Maximum Product Subarray](https://leetcode.com/problems/maximum-subarray/)
                                   Brute force is to check for each subarray and return the maximum product.This problem is similar to Maximum Sum Subarray(day2),with the difference that maximum product can also be obtained by current minimum multiplied by the array element since two negative numbers multiply to give a positive number.
So,we maintain a current max,current min and maximum then traverse the array and change their values accordingly.
2. [Triplet sum in an array](https://practice.geeksforgeeks.org/problems/triplet-sum-in-array-1587115621/1#) : The method to solve this problem in O(n) time Complexity is by using three pointers concept.Sort the array and place three pointers one at start,other one position ahead of first pointer and the third one at end position, then find out the sum of values pointed by these pointers if it is equal return else if value is less than the key that means some value must be reduced so that sum becomes equal since array is sorted third pointer is decremented and same goes for sum greater than key.
             
**Link(s) to work**
1. [Maximum Product Subarray](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day4_a.cpp)
2. [Triplet sum in an array](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day4_b.cpp)\


[Post on twitter](https://twitter.com/pundhir_rakhi/status/1454503615062687745)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day4-100daysofcode-100daysofdsa-activity-6860268067155529728-yij6)

### Day 5: October 31, Sunday

**Today's Progress**: Problem : [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/)
                               This is one of the most important problems of dsa.It can be solved in O(n) time complexity and O(n) space complexity using two auxiliary arrays -                      left and right.Water can be stored at any position only if there is a tower of greater height to its left as well as to its right.So, we maintain left array to store maximum height to left of any position and right array to store maximum height to right of any position.Then,amount of water stored at any index will be minimum of left height and right height at that index.Since tower at any index will also cover some space so we have to subtract height at that index from the minimum value.
             
**Link(s) to work**
1. [Trapping Rain /water](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day5.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1454871631168294914)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day5-100daysofcode-100daysofdsa-activity-6860636142484770816-jQBJ)

### Day 6: November 1, Monday

**Today's Progress**: Problem : [Merge Intervals](https://leetcode.com/problems/merge-intervals/)
                              To solve this problem we have to maintain two pointers one that traverses the array and compares the start time of any interval with the end time                                 of previous interval,if it is less, then swap that with the value pointed by the first pointer else increment the first pointer.
             
**Link(s) to work**
1. [Merge Intervals](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day6.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1455224568793079811)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day6-100daysofcode-100daysofcodechallenge-activity-6860988895635632128-AaVS)

### Day 7: November 2, Tuesday

**Today's Progress**: Problem : [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/)
                              To solve this problem we have to traverse the array once and find the minimum day to buy a stock then check for a day so that the profit obtained                                 is maximum.We will maintain a min variable to store minimum value day if a day is greater than this min variable implies that we can now look for a day to sell stocks so we calculate the profit and store it to compare it further.
             
**Link(s) to work**
1. [Best Time to Buy and Sell Stock](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day7.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1455596285457666049)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day7-100daysofcode-100daysofcodechallenge-activity-6861361156280459264-MZc1)

### Day 8: November 3, Wednesday

**Today's Progress**: Problem : [Median of two sorted arrays of different size](https://leetcode.com/problems/median-of-two-sorted-arrays/)
                                An optimal approach to solve this problem is to merge both the arrays into the first arrays (so that no extra space is used) and then calculate for the median. To calculate for median-(if size of array(n) is an odd number) median=(n+1)/2 th element of array, and (if the size of array(n) is an even number) median =average of ((n/2)th array element and (n/2+1)th array element). So, this problem included math and merging two sorted arrays into one sorted array without using any extra space.
             
**Link(s) to work**
1. [Median of two sorted arrays of different size](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day8.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1455596285457666049)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day7-100daysofcode-100daysofcodechallenge-activity-6861361156280459264-MZc1)


             
