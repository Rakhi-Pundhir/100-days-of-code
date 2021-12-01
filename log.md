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
                                An optimal approach to solve this problem is to merge both the arrays into the first array (so that no extra space is used) and then calculate for the median. To calculate for median-(if size of array(n) is an odd number) median=(n+1)/2 th element of array, and (if the size of array(n) is an even number) median =average of ((n/2)th array element and (n/2+1)th array element),keep in mind the indexing of array. So, this problem included math and merging two sorted arrays into one sorted array without using any extra space.
             
**Link(s) to work**
1. [Median of two sorted arrays of different size](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day8.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1455928286144393222)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day8-100daysofcode-100daysofcodechallenge-activity-6861694973352538112-do6F)

### Day 9: November 4, Thursday

**Today's Progress**: Problem : [Majority Element II](https://leetcode.com/problems/majority-element-ii/)
                              Question-Given an integer array of size n, find all elements that appear more than ⌊ n/3 ⌋ times. I never knew how easily this question could be done using C++ STL(here, maps) all we need to do is create a map and fill in the values with their frequency. Then extract values from map and store those elements in an answer vector whose frequency or count is more than the given ratio(size of given array/k).
                                              
**Link(s) to work**
1. [Majority Element II](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day9.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1456310014251921409)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day9-100daysofcode-100daysofdsa-activity-6862075019711905792-sdD7)

### Day 10: November 5, Friday

**Today's Progress**: Problem : [Factorial of Large Number](https://practice.geeksforgeeks.org/problems/factorials-of-large-numbers2508/1)
.                               To store large factorials int cannot be used so we take a vector/array to store digits of factorial,initialize it with 1 and using basic math we multiply i (from 2 till the given number) with each digit of the factorial obtained so far taking care of the carry generated. The fact is that these digits will be stored in reverse order and finally we return the reverse of the array.In Java we can use Big Integer for storing large factorials.Here, we could also use linked list.
                                              
**Link(s) to work**
1. [Factorial of Large Number](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day10.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1456685105049575425)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day10-100daysofcode-100daysofdsa-activity-6862450041106366464-fThe)

### Day 11: November 6, Saturday

**Today's Progress**: Problem : [Spiral Matrix](https://leetcode.com/problems/spiral-matrix/)
.                              We have to return elements of a matrix in spiral form and for this we need to take four pointers for row start,row end,column start and column end each. Then start traversing the array starting with the first row and pushing elements from column start to column end into an answer vector. Now, we have to traverse the last column(to maintain spiral form) from row start to row end, then the last row from column end to column start and finally the first row starting from row end to row start.We continue this till all elements are printed.One important thing to note here is that we have to update the four pointers after each operation i.e. row start is incremented by one after we have traversed the first row and column end is decremented by one after traversing the last column and so on. 
                                              
**Link(s) to work**
1. [Spiral Matrix](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day11.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1457040567330738179)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day11-100daysofcode-100daysofdsa-activity-6862807084292042752-hZLK)

### Day 12: November 7, Sunday

**Today's Progress**: Problem : [Search a 2D Matrix](https://leetcode.com/problems/search-a-2d-matrix/)
.                               We have to search for an element in a 2D Matrix in which the elements of each row are sorted and the first integer of each row is greater than the last integer of the previous row. So, we check if our target value is less than the first integer of the current row then it cannot be present in the matrix and if the target value is greater than the last integer of the current row that means it is present in the next row else that target might be present in the current row so we use binary search on the current row(given elements of each row are sorted) if target is found we return true else if not found we return false.
                                              
**Link(s) to work**
1. [Search a 2D Matrix](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day12.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1457399344659791875)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day12-100daysofcode-100daysofdsa-activity-6863165716204531712-KZd1)

### Day 13: November 8, Monday

**Today's Progress**: Problem : [Rotate 2D Matrix by 90 degrees](https://leetcode.com/problems/rotate-image/)
.                               We have to rotate elements of a 2D matrix in-place so, we first transpose the matrix and then reverse elements of each row.To transpose the 2D vector we use two for loops(nested loops) one(i) from 0 to size of matrix -1 and the other loop(j) from 0 to i. Then, swap elements of matrix[i][j] with matrix[j][i]. Finally we reverse elements of each row to get a rotated matrix.
                                              
**Link(s) to work**
[Rotate 2D Matrix by 90 degrees](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day13.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1457710850005889030)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day13-100daysofcode-100daysofdsa-activity-6863477323472232448-BEZP)

### Day 14: November 9, Tuesday

**Today's Progress**: Problem : [Count triplets with sum less than given sum](https://practice.geeksforgeeks.org/problems/count-triplets-with-sum-smaller-than-x5549/1)
.                               Given an array count number of triplets having sum smaller than the given sum. The idea is to sort the given array and use three pointers approach for searching the triplets.Start traversing the array and find out the sum of the values pointed by the three pointers. If the sum is lgreater or equal to the given value decrement the pointer at the end by one(to make sum value smaller as array is sorted) else increment count and second pointer,also, we have to increment count by (k-j)
till the sum value is smaller than the given sum.
                                              
**Link(s) to work**
[Count triplets with sum less than given sum](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day14.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1458036917379874824)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day14-100daysofcode-100daysofdsa-activity-6863803016231960576-ruhB)

### Day 15: November 10, Wednesday

**Today's Progress**: Problem : [Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/)
                             Given the head of a singly linked list we have to return the list after reversing it.A reversed linked list means that the head will point to the last node of the original list and the next field of every node will contain address of the previous node so that we can traverse the list in reverse order.So,for this we use three pointers-one that will traverse the list in the forward direction(nextnode), second to store address of previous node so that we can assign it to the current node and the third one will point to the current node on which we have to perform reverse operation.We will then traverse the complete list and update these pointers accordingly.
                                              
**Link(s) to work**
[Reverse Linked List](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day15.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1458467024313540611)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day15-100daysofcode-100daysofdsa-activity-6864233490024673280-YY7s)

### Day 16: November 11, Thursday

**Today's Progress**: Problem : [Detect cycle in Linked List](https://leetcode.com/problems/linked-list-cycle/)
                                Given the head of a linked list, determine if the linked list has a cycle in it.A linked list has cycle if next field of two nodes point to the same node and we can detect this cycle or loop by using hare and tortoise algorithm.We take two pointers fast(hare) and slow(tortoise) pointing to the haed node of the linled list.Then we move both the pointers slow moves by one step and fast moves by two steps and we continue this fast and slow points to the same node or else we have traversed the complete list.
                                              
**Link(s) to work**
[Detect cycle in Linked List](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day16.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1458812618370551813)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day16-100daysofcode-womenwhocode-activity-6864576490684719104-6iAV)

### Day 17: November 12, Friday

**Today's Progress**: Problem : [Find loop node in Linked List](https://leetcode.com/problems/linked-list-cycle-ii/)
                                Given the head of a linked list find the node where the cycle or loop starts in the list,if present.We use the idea to detect cycle in a list i.e. by using hare and tortoise algorithm,if there is a cycle in the list,fast and slow pointers would point to the same node at that point we move one of the two pointers to head node and again run a loop and this time both the pointers move by one step and we end the loop when we reach a common node that is pointed by both the pointers-fast and slow and return that common node.
                                              
**Link(s) to work**
[Find loop node in Linked List](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day17.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1459191680834310152)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day17-100daysofcode-100daysofdsa-activity-6864956461315952640-w2mv)

### Day 18: November 13, Saturday

**Today's Progress**: Problem : [Remove duplicates from sorted linked list](https://leetcode.com/problems/remove-duplicates-from-sorted-list/)
                                Given the head of a sorted linked list remove all duplicate lements and return the sorted list. So, for this we maintain two pointers one for the current node and the other that traverses the list and then compare values pointed by both the nodes.If equal then the address or next field of the current node should point to the address field of nextnode's address so that the duplicated value is removed and incase the values are not equal we simply move the two pointers.
                                              
**Link(s) to work**
[Remove duplicates from sorted linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day18.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1459584553320730628)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day18-100daysofcode-100daysofdsa-activity-6865350777075048448-Ysn4)

### Day 19: November 14, Sunday
 
**Today's Progress**: Problem : [Remove duplicates from an unsorted linked list](https://practice.geeksforgeeks.org/problems/remove-duplicates-from-an-unsorted-linked-list/1#)
                                Given the head of an unsorted linked list we have to return the list after removing the duplicate elements.This problem is very easy if you try  solving it using sets of C++ STL.I have used an unordered set here to compare for duplicated elements since a set can only have unique elements.So,we maintain two pointers one that traverses the list and check for duplicate elements and the other to maintain the list with only unique elements.
                                              
**Link(s) to work**
[Remove duplicates from sorted linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day19.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1459943649890869248)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day19-100daysofcode-100daysofdsa-activity-6865709946336608256-uT65)

### Day 20: November 15, Monday
 
**Today's Progress**: Problem : [Middle of the linked list](https://leetcode.com/problems/middle-of-the-linked-list/)
                                Given the head of a singly linked list, return the middle node of the linked list.If there are two middle nodes, return the second middle node.
                                This is quite simple just use fast and slow pointers method.The fast and slow pointers initially point to the head node of the linked list.Then, move slow by one step forward and fast by two steps forward and when fast pointer reaches the end of the linked list our slow pointer would be right at the middle element of that linked list.In case head node is NULL i.e. the list is empty or if it contains only one node then simply return the head pointer. 
                                              
**Link(s) to work**
[Middle of the linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day20.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1460306036389072896)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day20-100daysofcode-100daysofdsa-activity-6866072163519225857-Zwep)

### Day 21: November 16, Tuesday
 
**Today's Progress**: Problem : [Nth node from end of linked list](https://practice.geeksforgeeks.org/problems/nth-node-from-end-of-linked-list/1#)
                                Given a linked list consisting of L nodes and given a number N. The task is to find the Nth node from the end of the linked list.Since there is no previous address field in a singly linked list we have to find the node from the front of the linked list instead of finding it from the end of the list.For this, we have to calculate the length of the linked list using a counter varible and increment it as we traverse the list.Then taking the difference of length of list and position of node we can find out the node.
                                              
**Link(s) to work**
[Nth node from end of linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day21.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1460670877469528066)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day21-100daysofcode-100daysofdsa-activity-6866437230441967616-Bud7)

### Day 22: November 17, Wednesday
 
**Today's Progress**: Problem : [Reverse a doubly linked list](https://practice.geeksforgeeks.org/problems/reverse-a-doubly-linked-list/1)
                                Given a doubly linked list of n elements. The task is to reverse the doubly linked list.The idea is to simply reverse the address fields of every node i.e. we have to swap previous and next fields so as to get a reversed list since a doubly linked list also has access to the previous node.Also,we have to traverse the list using the updated previous field of the node which now contains the addresss to the next node of the list.
                                              
**Link(s) to work**
[Reverse a doubly linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day22.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1461028946502320141)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day22-100daysofcode-100daysofdsa-activity-6866795258974470144-cpo3)

### Day 23: November 18, Thursday
 
**Today's Progress**: Problem : [Check for circular linked list](https://practice.geeksforgeeks.org/problems/circular-linked-list/1#)
                                Problem Statement : Given head, the head of a singly linked list, find if the linked list is circular or not. A linked list is called circular if it not NULL terminated and all nodes are connected in the form of a cycle. An empty linked list is considered as circular.If there is a circular linked list the last node would point to the head node so we simply have to traverse the list until head becomes equal to temp(pointer used to traverse the list) and incase NULL is encountered at any point that would mean the linked list is not circular.
                                              
**Link(s) to work**
[Check for circular linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day23.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1461382470910177284)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day23-100daysofcode-womenwhocode-activity-6867147381142622208-ihbA)

### Day 24: November 19, Friday
 
**Today's Progress**: Problem : [Intersection point of two linked list](https://leetcode.com/problems/intersection-of-two-linked-lists/)
                                Given the heads of two singly linked-lists headA and headB, return the node at which the two lists intersect. If the two linked lists have no intersection at all, return null.The idea is to traverse both the list until we reach a common node or else return null if any of the list terminates(case when there is no intersection) but to compare we have to start traversing the lists from same length.For this we calculate the difference between lengths of both the lists and then traverse the longer list first until the difference becomes zero, at this point we can start traversing both the lists together and compare for a common node.
                                              
**Link(s) to work**
[Intersection point of two linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day24.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1461748678780018689)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day24-100daysofcode-womenintech-activity-6867514948818493440-CKYG)

### Day 25: November 21, Sunday
 
**Today's Progress**: Problem : [Check if linked list is palindrome](https://leetcode.com/problems/palindrome-linked-list/)
                                Given the head of a singly linked list, return true if it is a palindrome.Not making this too complicated but we can use recursion to traverse the linked list in back direction since a singly linked list has only a next address field.Then, we simply compare the values from start with that of end and move start pointer by one using next field and end pointer by one step backwards using recursion.If at any point (before we have reached NULL) the values are not equal we return false.
                                              
**Link(s) to work**
[check if linked lsit is palindrome](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day25.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1462428897987874820)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day25-100daysofcode-100daysofdsa-activity-6868195228218720256-1-93)


### Day 26: November 22, Monday
 
**Today's Progress**: Problem : [Sort linked list of 0,1 and 2](https://practice.geeksforgeeks.org/problems/given-a-linked-list-of-0s-1s-and-2s-sort-it/1#)
                                Given a linked list of N nodes where nodes can contain values 0s, 1s, and 2s only.The task is to segregate 0s, 1s, and 2s linked list such that all zeros segregate to head side, 2s at the end of the linked list, and 1s in the mid of 0s and 2s.The idea is to store count of all 0's,1's and 2's in an array and then traverse the list and overwrite the values with 0's first till its count becomes zero in the array and same operation for 1's and 2's.
                                              
**Link(s) to work**
[Sort linked list of 0,1 and 2](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day26.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1462834915255357451)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day26-100daysofcode-100daysofdsa-activity-6868599863781789696-eR2z)

### Day 27: November 23, Tuesday
 
**Today's Progress**: Problem : [Flatten linked list](https://practice.geeksforgeeks.org/problems/flattening-a-linked-list/1)
                                Given a Linked List of size N, where every node represents a sub-linked-list and contains two pointers:
(i) a next pointer to the next node,
(ii) a bottom pointer to a linked list where this node is head.
Each of the sub-linked-list is in sorted order.
Flatten the Link List such that all the nodes appear in a single level while maintaining the sorted order. 
Note: The flattened list will be printed using the bottom pointer instead of next pointer.
This problem is divided into sub problems to merge two sorted linked list where first list is pointed by the head pointer and another by head->next pointer.Since we have to merge two lists starting from the end we use recursion to reach the end and then keep on merging the lists till we get one sorted list.For that we take a dummy node and pointers to the lists and this node then, we traverse both the lists and compare the values just as we had done for merging sorted lists.
                                              
**Link(s) to work**
[Flatten linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day27.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1463206104221900805)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day27-100daysofcode-100daysofdsa-activity-6868971115105153024-0ah8)

### Day 28: November 24, Wednesday
 
**Today's Progress**: Problem : [Merge sort for linked list](https://leetcode.com/problems/sort-list/)
                                Given the head of a linked list, return the list after sorting it in ascending order.Merge sort for linked list is similar to merge sort for arrays.So,first we find mid of the list using slow and fast pointers then divide the list into two lists partitioning from the mid and then passing these lists to the merge function.Here, in the merge function the lists are compared for values and merged into one sorted list just as we do for merging of two sorted linked lists.
                                              
**Link(s) to work**
[Merge sort for linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day28.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1463537555802972163)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day28-100daysofcode-100daysofdsa-activity-6869302563150409728-wYdD)

### Day 29: November 25, Thursday
 
**Today's Progress**: Problem : [Add two linked lists](https://leetcode.com/problems/add-two-numbers/)
                                You are given two non-empty linked lists representing two non-negative integers. The digits are stored in reverse order, and each of their nodes contains a single digit. Add the two numbers and return the sum as a linked list.Take a dummy node and keep adding to it the nodes containing the sum which is actually mod of the sum also add carry to the sum which is division of the sum.
                                              
**Link(s) to work**
[Add two linked lists](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day29.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1463926067010277382)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day29-100daysofcode-100daysofdsa-activity-6869692025265098752-Gswb)


### Day 30: November 26, Friday
 
**Today's Progress**: Problem : [Reverse linked list in groups of k](https://practice.geeksforgeeks.org/problems/reverse-a-linked-list-in-groups-of-given-size/1#)
                                Given a linked list of size N. The task is to reverse every k nodes (where k is an input to the function) in the linked list. If the number of nodes is not a multiple of k then left-out nodes, in the end, should be considered as a group and must be reversed.This is similar to reversing linked list but here maintain a counter varible to count k groups.After reversing these k groups repeat this process till the end of the list and to continue this compare value of nextnode for NULL if nodes are left call this reverse function recursively.
                                              
**Link(s) to work**
[Reverse linked list in groups of k](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day30.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1464289452386250754)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day30-100daysofcode-freecode-activity-6870055545064321024-bN7J)

### Day 31: November 28, Sunday
 
**Today's Progress**: Problem : [Maximum depth of binary tree](https://leetcode.com/problems/maximum-depth-of-binary-tree/)
                                Given the root of a binary tree, return its maximum depth.A binary tree's maximum depth is the number of nodes along the longest path from the root node down to the farthest leaf node.Maximum depth is actually the height of the binary tree.To find this calculate height of left subtree and right subtree of the binary tree and take maximum of the two plus one (for the root node),this gives you the height or maximum depth of the binary tree.
                                              
**Link(s) to work**
[Maximum depth of binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day31.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1465009384048660483)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day31-100daysofcode-womenintech-activity-6870775427267465216-czWY)

### Day 32: November 29, Monday
 
**Today's Progress**: Problem : [Inorder traversal of binary tree](https://leetcode.com/problems/binary-tree-inorder-traversal/)
                                Given the root of a binary tree, return the inorder traversal of its nodes' values.In Inorder traversal we first print the left subtree nodes then the root vale and at last the right subtree nodes.So,for this we recursively call the inorder function and traverse left subtree storing its values in a vector and the the right subtree storing its values also in the vector.
                                              
**Link(s) to work**
[Inorder traversal of binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day32.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1465385333797785600)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day32-100daysofcode-100daysofdsa-activity-6871151358410682368-uXAG)

### Day 33: November 30, Tuesday
 
**Today's Progress**: Problem : [Balanced binary tree](https://leetcode.com/problems/balanced-binary-tree/)
                                Given a binary tree, determine if it is height-balanced.For this problem, a height-balanced binary tree is defined as:a binary tree in which the left and right subtrees of every node differ in height by no more than 1.The idea is to calculate height for left and right subtrees then find their difference if it is less than or equal to 1 return true else return false.
                                              
**Link(s) to work**
[Balanced binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day33.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1465736623388119041)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day33-100daysofcode-womenintech-activity-6871502540828241922-qhsu)

### Day 34: December 01, Wednesday
 
**Today's Progress**: Problem : [Level order traversal binary tree](https://leetcode.com/problems/binary-tree-level-order-traversal/)
                                Given the root of a binary tree, return the level order traversal of its nodes' values. (i.e., from left to right, level by level).To solve this problem we use queue data structure and insert root node in it.Now we can start the logic to print nodes level by level.We continue the following task until the queue becomes empty.We extract element at the front of the queue and print it then pop it from the queue.Also, we check for each printed node if it has left and right child and insert them into the queue. 
                                              
**Link(s) to work**
[Level order traversal binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day34.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1466069471831887873)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day34-100daysofcode-freecodecamp-activity-6871834567490322432-KWr8)


             
