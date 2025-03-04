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


### Day 35: December 03, Friday
 
**Today's Progress**: Problem : [Bottom up traversal of binary tree](https://leetcode.com/problems/binary-tree-level-order-traversal-ii/)
                                Bottom up traversal binary tree Given the root of a binary tree, return the bottom-up level order traversal of its nodes' values. (i.e., from left to right, level by level from leaf to root).This is similar to the level order traversal of binary tree.In level order traversal queue was used so here for reverse level order traversal we could've used a stack but the order changes so for that we have to use both queue and stack.Also,first right child will be pushed into the queue and then the left child to maintain the order from left to right as stated in the problem statement.At last we pop all elements of the stack into a vector and return it.
                                              
**Link(s) to work**
[Bottom up traversal of binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day35.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1466775851660242946)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day35-100daysofcode-womenintech-activity-6872540721094758400-eVC2)

### Day 36: December 04, Saturday
 
**Today's Progress**: Problem : [Right view of binary tree](https://leetcode.com/problems/binary-tree-right-side-view/)
                                Given the root of a binary tree, imagine yourself standing on the right side of it, return the values of the nodes you can see ordered from top to bottom.For the right view of binary tree we use level order traversal.Here, we take a queue and store nodes level wise in the queue.The right most nodes means the nodes that are present at the end of each level or at the end of queue so we push those nodes only into the answer vector.
                                              
**Link(s) to work**
[Right side view of binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day36.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1467193410306011136)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day36-100daysofcode-100daysofdsa-activity-6872958388926607360-48si)

### Day 37: December 05, Sunday
 
**Today's Progress**: Problem : [Lowest common ancestor of binary tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree/)
                                The lowest common ancestor is defined between two nodes p and q as the lowest node in T that has both p and q as descendants. Here, when left and right of root node both are not equal to NULL that is our LCA else we make recursive calls to get that.
                                              
**Link(s) to work**
[Lowest common ancestor of binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day37.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1467542047552798726)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day37-100daysofcode-womenintech-activity-6873308153971396608--qHf)

### Day 38: December 06, Monday
 
**Today's Progress**: Problem : [Invert binary tree](https://leetcode.com/problems/invert-binary-tree/)
                                Given the root of a binary tree, invert the tree, and return its root.Here,we have to convert the given binary tree into a tree that is mirror image of this tree.If we break the problem into subproblems and try to invert only the root node then it is clearly understood that we only have to swap the left and right child nodes of the parent node.So,to invert the complete tree we make recursive calls for left and right subtrees performing the same operation for all subproblems.
                                              
**Link(s) to work**
[Invert binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day38.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1467890255017570305)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day38-100daysofcode-womenwhocode-activity-6873654790195429376-oJdR)

### Day 39: December 07, Tuesday
 
**Today's Progress**: Problem : [Diameter of binary tree](https://leetcode.com/problems/diameter-of-binary-tree/)
                                Given the root of a binary tree, return the length of the diameter of the tree.Diameter is the longest path between any two leaf nodes in the binary tree.If the diameter passes through root node then length of diameter will be (height of left subtree+height of right subtree+1) one for the root node,this is when the path requires nodes and not edges and incase the diameter does not pass through the root node then, we will take maximum of the left and right diameter.
                                              
**Link(s) to work**
[Diameter of binary tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day39.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1468275414212571139)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day39-100daysofcode-womenintech-activity-6874039695551164416-x7oS)

### Day 40: December 08, Wednesday
 
**Today's Progress**: Problem : [search in a binary search tree](https://leetcode.com/problems/search-in-a-binary-search-tree/)
                                You are given the root of a binary search tree (BST) and an integer val.Find the node in the BST that the node's value equals val and return the subtree rooted with that node. If such a node does not exist, return null.A binary search tree is whose left child node is lesser than root node and right child node is greater than the root node or parent node.So we compare it with the root node if equal we return that node,in case key is greater than root we search for it in the right subtree and if lesser than root we search for it in the left subtree.
                                              
**Link(s) to work**
[Search in a binary search tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day40.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1468601068091101184)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day40-100daysofcode-freecodecamp-activity-6874365979976171520-a_do)

### Day 41: December 09, Thursday
 
**Today's Progress**: Problem : [Delete in a binary search tree](https://leetcode.com/problems/delete-node-in-a-bst/)
                                Given a root node reference of a BST and a key, delete the node with the given key in the BST.If the node to be deleted is lesser than root node, search for it in the right subtree, and if it is greater, then do the same in left subtree.Now,while deleting any node we have to check for the following three cases-if the node to be deleted is a leaf node then simply delete it, if the node to be deleted has only one child then replace it with that child and delete, and if it has both left and right child then replace the node to be deleted by its inorder successor(which incase of a BST is the last node in the right subtree of that particular node) and also delete the repeated value generated after replacing.
                                              
**Link(s) to work**
[Delete in a binary search tree](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day41.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1468963151706157067)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day41-100daysofcode-womenintech-activity-6874728018997252096-2Yvw)

### Day 42: December 10, Friday
 
**Today's Progress**: Problem : [Construct binary search tree from preorder traversal](https://leetcode.com/problems/construct-binary-search-tree-from-preorder-traversal/)
                                Given an array of integers preorder, which represents the preorder traversal of a BST (i.e., binary search tree), construct the tree and return its root.Start with creating the root node with the first element of array(containing preorder traversal) then we can make recursive calls to the build tree function and insert other nodes maintaining the property of a binary search tree.If the element to be inserted is lesser than root value we call for the function to insert it to the left of root and do same for the right side of root.When there is space(NULL) for inserting the node,create a newnode and assign that value to it and return its address to the parent node. 
                                              
**Link(s) to work**
[Construct binary search tree from preorder traversal](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day42.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1469316019009187840)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day42-100daysofcode-freecodecamp-activity-6875080970232578048-EtTQ)

### Day 43: December 11, Saturday
 
**Today's Progress**: Problem : [Reverse a string using Stack](https://practice.geeksforgeeks.org/problems/reverse-a-string-using-stack/1#)
                                You are given a string S, the task is to reverse the string using stack.Since a stack follows LIFO(Last In First Out) principle,we can use it to reverse a string by storing each character of the string into the stack and then empty the stack so that the last character comes out first.Then store the popped out characters in any string or into the same string starting from the first index and incrementing it gradually. 
                                              
**Link(s) to work**
[Reverse a string using Stack](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day43.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1469698974462271491)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day43-100daysofcode-freecodecamp-activity-6875464096821612544-o6kr)


### Day 44: December 12, Sunday
 
**Today's Progress**: Problem : [Sort a Stack in descending order](https://practice.geeksforgeeks.org/problems/sort-a-stack/1#)
                                Given a stack, the task is to sort it such that the top of the stack has the greatest element.To sort it in this order all we have to keep in mind is that the top of stack must point to the greatest element.so, for this we first empty the stack and then insert elements into it one by one.If the stack is empty simply push the value onto the stack.Also, if the value to be inserted is greater than the top of stack we can push it onto the stack since in that case our top would have the greatest element only.But in case the value to be added is lesser than the top we have to first pop out hte value and then insert our lower element into the stack and after that only we can now insert the popped element back to the stack and continue this process till all elements have been inserted(recursive calls to all functions are completed).
                                              
**Link(s) to work**
[Sort a Stack in descending order](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day44.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1470057626842976257)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day44-100daysofcode-freecodecamp-activity-6875823648536690688--RXo)

### Day 45: December 13, Monday
 
**Today's Progress**: Problem : [Valid Parentheses](https://leetcode.com/problems/valid-parentheses/)
                                Given a string s containing just the characters '(', ')', '{', '}', '[' and ']', determine if the input string is valid.An input string is valid if: Open brackets must be closed by the same type of brackets and also,open brackets must be closed in the correct order.So we have to traverse the string and insert each opening bracket into the stack of characters.And if the character is a closed bracket check the top of stack for the same type of open bracket,if so pop it out of stack and continue for other characters of string.If not return false also, in the end if the stack is not empty return false since this means that the number of opening brackets were not equal to the number of closing brackets.
                                              
**Link(s) to work**
[Valid Parentheses](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day45.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1470448941212717056)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day45-100daysofcode-freecodecamp-activity-6876213938376192001-Qaj1)


### Day 46: December 15, Wednesday
 
**Today's Progress**: Problem : [evaluation of postfix expression](https://practice.geeksforgeeks.org/problems/evaluation-of-postfix-expression1735/1#)
                                Given string S representing a postfix expression, the task is to evaluate the expression and find the final value. Operators will only include the basic arithmetic operators.Here, we create a stack of integers and insert only digits(0-9) into it while traversing the string.In case the charater is not a digit but is an operator we pop the topmost two numbers of stack and perform arithmetic operations on them based on the oerator and push the result of the operation into the stack and continue this process till we reach end of the given string.At last, the final output will be the value at the top of the stack.
                                              
**Link(s) to work**
[evaluation of postfix expression](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day46.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1471162914732085253)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day46-100daysofcode-freecodecamp-activity-6876927580314865665-Efft)

### Day 47: December 16, Thursday
 
**Today's Progress**: Problem : [The Celebrity Problem](https://practice.geeksforgeeks.org/problems/the-celebrity-problem/1)
                                If you go to a party of N people, find if there is a celebrity in the party or not. A square NxN matrix M[][] is used to represent people at the party such that if an element of row i and column j  is set to 1 it means ith person knows jth person.This is the most interesting problem I have ever solved where a man becomes the celebrity if he does not know anyone and there could be no person who does not know him.So,for this we use a stack to store the index of all people and also the celebrity number.Then pop out two topmost elements of stack and check for two conditions-if i know j then j can be a celebrity so push j into stack or if i does not know j then i could be a celebrity so push i into stack.Repeat this till stack size becomes less than 2,then the stack would contain only one number which maybe the celebrity and to check this one we compare it with each index,incase this person knows someone or there is someone who doesn't know him then he can't be the celebrity else return this person number.
                                              
**Link(s) to work**
[The Celebrity Problem](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day47.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1471528915134922752)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day47-100daysofocde-womenintech-activity-6877295047595855874-bnXa)

### Day 48: December 19, Sunday
 
**Today's Progress**: Problem : [The Circular Tour](https://practice.geeksforgeeks.org/problems/circular-tour/1#)
                                Suppose there is a circle. There are N petrol pumps on that circle. You will be given two sets of data.
1. The amount of petrol that every petrol pump has.
2. Distance from that petrol pump to the next petrol pump.
Find a starting point where the truck can start to get through the complete circle without exhausting its petrol in between.For this we have to keep a fuel variable and a required fuel variable to keep track of the amount of fuel needed to go from one station to another.If it is not possible then later we could perform it using existing fuel plus the fuel received at that particular station.

                                              
**Link(s) to work**
[The Circular Tour](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day48.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1472619666979766276)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day48-100daysofcode-womenintech-activity-6878384804727988224-tzbz)

### Day 49: December 20, Monday
 
**Today's Progress**: Problem : [Valid Substring](https://practice.geeksforgeeks.org/problems/valid-substring0624/1)
                                Given a string S consisting only of opening and closing parenthesis 'ie '('  and ')', find out the length of the longest valid(well-formed) parentheses substring.NOTE: Length of the smallest valid substring ( ) is 2.We traverse the string and push each opening bracket into a stack of characters.On encountering any closed bracket first we check if the top of stack is a open bracket if so it would make a pair of a valid substring and so increment the count variable by 2 and pop it from the stack,in all other cases simply move on to the next character of the given string.

                                              
**Link(s) to work**
[Valid Substring](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day49.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1472982469561384967)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day49-100daysofcode-freecodecamp-activity-6878747702990036992-xqJ5)


### Day 50: December 23, Thursday
 
**Today's Progress**: Problem : ##Create graph using adjacency matrix
                                Input the number of vertices and the number of edges of the graph.Create a 2-D array/matrix and fill in all the values with 0.Then input all edges and fill those indexes with 1 that have an edge in between.If it is an undirected graph value at index [i][j] will be 1 and also value at index [j][i] will be 1 and for a directed graph value at [i][j] only will be 1.Time complexity is v * v where v is the number of vertices in the graph.

                                              
**Link(s) to work**
[Create a graph using adjacency matrix](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day50.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1474006789024731137)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day50-100daysofcode-freecodecamp-activity-6879771681292918784-1yUZ)

### Day 51: December 24, Friday
 
**Today's Progress**: Problem : ##Create graph using adjacency list
                                Input the number of vertices and the number of edges of the graph.Create an array of vectors.Then input the edges and fill in these edges in their specified vertices.For a directed graph edge is unidirectional and for an undirected graph it is bidirectional.

                                              
**Link(s) to work**
[Create a graph using adjacency list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day51.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1474418486793306117)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day51-100daysofcode-womenwhocode-activity-6880183776102670336-Ncqc)

### Day 52: December 25, Saturday
 
**Today's Progress**: Problem : ##Detect cycle in a graph
                                Input the number of vertices and the number of edges.Declare a visited array with initial values as 0 i.e. no node is visited and as we encounter any node we change its visited state from 0 to 1.We start with a source node and visit all its edges.In case any of the node is visted already and also it is not that node's parent that indicated there is a cycle in the graph. 

                                              
**Link(s) to work**
[Detect cycle in a graph](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day52.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1474771591842041858)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day52-100daysofcode-freecodecamp-activity-6880536649038647296-H7QY)

### Day 53: December 27, Monday
 
**Today's Progress**: Problem : ##Breadth First Search in a graph
                                Assign a status 0 to all nodes and push source node into a queue and change its status to 1.Then pop an element from the queue and visit all its neighbours and push only those nodes in the queue with a status equal to 0 and again pop an element from queue, continue this till the destination is reached or when the queue becomes empty.Trace the path that led to the destination node and this will be our shortest path from source to that node.

                                              
**Link(s) to work**
[Breadth First Search in a graph](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day53.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1475514090407673857)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day53-100daysofcode-codingdays-activity-6881278374644355072-ZE9x)

### Day 54: December 28, Tuesday
 
**Today's Progress**: Problem : ##Depth First Search in a graph
                                Assign a status 0 to all nodes and push source node into a stack then pop it.Now, this node is processed so change its status to 1 and visit all its neighbours and push those nodes only with status equal to 0.Then again pop an element from stack and repeat this till the stack becomes empty.

                                              
**Link(s) to work**
[Depth First Search in a graph](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day54.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1475888013401939969)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day54-100dasyofcode-freecodecamp-activity-6881653140005904384-4rYK)

### Day 55: December 31, Friday
 
**Today's Progress**: Problem : ##Floyd Warshall Algorithm
                                Floyd warshall algorithm is used to find the shortest distance between every pair of nodes in a weighted directed graph using the idea to traverse the distance by bringing an intermediate node in between the two nodes.

                                              
**Link(s) to work**
[Floyd Warshall Algorithm](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day55.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1476830254626869251)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day55-100daysofcode-freecodecamp-activity-6882595669970837504-o-yt)

### Day 56: January 01, Saturday
 
**Today's Progress**: Problem : ##Detect cycle in undirected graph
                                We start with traversing the graph and in case a node is already visited earlier and is not the parent then there exits a cycle.

                                              
**Link(s) to work**
[Detect cycle in undirected graph](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day56.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1477338942051524609)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day56-100daysofcode-freecodecamp-activity-6883104343042625536-uYPf)

### Day 57: January 02, Sunday
 
**Today's Progress**: Problem : [Count subarrays with product less than k](https://practice.geeksforgeeks.org/problems/count-the-subarrays-having-product-less-than-k1708/1/)
                                 We can use nested loops and form all subarrays then compare which subarray gives product less than k but time complexity would then be n squared so we optimize this using sliding window method.We calculate the product of elements in the window then move the window by one element, if product now becomes equal or greater than k we move the left point of the window and delete its entry by division else we add the number of elements in the answer variable and move the right point of the window.

                                              
**Link(s) to work**
[Count subarrays with product less than k](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day57.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1477703491548106753)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day57-100daysofcode-freecodecamp-activity-6883468668206907392-nYIj)

### Day 58: January 03, Monday
 
**Today's Progress**: Problem : [Number following a pattern](https://practice.geeksforgeeks.org/problems/number-following-a-pattern3126/1#)
                                 We can use stack to solve this problem.Here, we are making splits at each I encountered and then reverse the count for each D.Create a stack of characters and as you traverse the string push a number initialized with 1 into it and increase it by 1 and for each I do the same but also pop all elements from stack and add to the answer string.At last push the number and pop all.

                                              
**Link(s) to work**
[Number following a pattern](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day58.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1477925468330348544)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day58-100daysofcode-freecodecamp-activity-6883690674454044672-C7d_)


### Day 59: January 04, Tuesday
 
**Today's Progress**: Problem : [Decode the string](https://practice.geeksforgeeks.org/problems/decode-the-string2444/1)
                                 We are using a stack of characters to push each element of string except ']' as on encountering this character we have to start decoding the string.We will pop all characters out of stack until we get an opening bracket and then add the popped characters to an empty string and push it into the stack and then we will use a loop to multiply that string to itself k times.At last we will pop all characters from stack and add them to an empty answer string and then return it.

                                              
**Link(s) to work**
[Decode the string](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day59.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1478431934032199681)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day59-100daysofcode-freecodecamp-activity-6884197061445591042-hAuv)

### Day 60: January 05, Wednesday
 
**Today's Progress**: Problem : [Program to find Nth Ugly Number](https://practice.geeksforgeeks.org/problems/ugly-numbers2254/1/)
                                We are using dynamic programming to find an efficient solution for this problem.We keep on storing the ugly numbers in an array by choosing the minimum of three factors that are multiples of 2,3 or 5.Then we increment the pointer which gives the minimum factor to be stored as an ugly number.

                                              
**Link(s) to work**
[Program to find Nth Ugly Number](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day60.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1478750722384547840)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day60-100daysofcode-freecodecamp-activity-6884517235948306432-6VXr)


### Day 61: January 06, Thursday
 
**Today's Progress**: Problem : [Sliding Window Maximum](https://practice.geeksforgeeks.org/problems/maximum-of-all-subarrays-of-size-k3101/1)
                                We have to just find the maximum of all subarrays here and for that we will use sliding window method.We start with the first index and increment it until we get the size of window given in the question.Till window size is less than k we keep pushing the elements for future use in a queue to get another maximum incase the window slides and earlier maximum element is not included now.So, when the size hits we calculate our maximum present at front and then remove it calculations from queue if this gave the maximum value then we slide the window.Finally, the maximum of all windows will lie on the front of this queue.

                                              
**Link(s) to work**
[Sliding Window Maximum ](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day61.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1479812117473619972)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day61-100daysofcode-freecodecamp-activity-6885576933820645376-ECsh)


### Day 62: January 07, Friday
 
**Today's Progress**: Problem : [Longest Mountain](https://leetcode.com/problems/longest-mountain-in-array/)
                                We use peak and valley method here.We start counting for peak and valley once we get a peak ie. a value is lesser than its succeeding value.Till the time it is so we keep peak as true ans move on and till we get a valley i.e. a value is greater than its succeeeding value we keep valley as true and move on.In case we get both peak and valley as true at the same time it means we have covered a mountain so we then calculate its length and compare it with initial length of an mountain.

                                              
**Link(s) to work**
[Longest Mountain](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day62.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1479813514579513344)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day62-100daysofcode-freecodecamp-activity-6885578582651879424-j29H)

### Day 63: January 08, Saturday
 
**Today's Progress**: Problem : [Rotten Oranges](https://leetcode.com/problems/rotting-oranges/)/
                                We will be using BFS technique to traverse all adjacent oranges of any rotten orange.We start with pushing all rotten oranges into the queue then pop them one by one and visit their adjacent cells, if the cell contains a fresh orange(1) push it to the queue and mark it as rotten(2), when the queue becomes empty, stop.Then check if the total number of oranges(calculated by traversing the matrix) is equal to the number of oranges pushed into queue(since queue has only rotten oranges) then return time(incremented after processing oranges at a time) else return -1(i.e. it is impossible to rot all fresh oranges).Also, to calculate or visit nodes of a rotten orange we have used the concept of calculating next row and column by adding the row number or column number to the existing number.
                                              
**Link(s) to work**
[Rotten Oranges](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day63.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1480552092901072896)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day63-100daysofcode-freecodecamp-activity-6886317154505916416-h6RF)

### Day 64: January 09, Sunday
 
**Today's Progress**: Problem : [Delete N nodes after M nodes of a linked list](https://practice.geeksforgeeks.org/problems/delete-n-nodes-after-m-nodes-of-a-linked-list/1)/
                                We take a pointer initialize it with the head and traverse the linked list.We also maintain a counter variable which is zero initially and increment it as we move forward in the list.Till our counter variable is not equal to M we increment temp and when it becomes equal to M we have to delete N nodes from that point.To delete N nodes we simply change the address in the next field of prevoius node with the address mentioned in the Nth node.After this, we put the counter variable to zero again so that we can again count the M nodes to be skipped.

                                              
**Link(s) to work**
[Delete N nodes after M nodes of a linked list](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day64.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1482328776990412803)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day64-100daysofcode-freecodecamp-activity-6888092166787219456-4Tpa)

### Day 65: January 10, Monday
 
**Today's Progress**: Problem : overlapping rectangles
                                We can find all points and check if they lie inside the other rectangle or not but feasible will be to check for those conditions when the two rectangles will not overlap. These are - when a rectangle is above the other rectangle ( check this using the y coordinates ) and when a rectangle is to the left of the other rectangle ( check this using the x coordinates ) Also check if either rectangle is just a line.
                                              
**Link(s) to work**
[overlapping rectangles](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day65.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1482329648185094152)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day65-100daysofcode-freecodecamp-activity-6888092458312335360-eqH9)

### Day 66: January 11, Tuesday
 
**Today's Progress**: Problem : run length encoding
                                We traverse the string and count the occurences of every character then append that string character and its count to the result string then return it. OR We can make use of maps in STL. Create a map with characters as keys and integer as values then insert each characeter of the string into it and increment the count of that key as you traverse the string and encounter it.At last pop all key value pairs and append them to an empty string,use to_string function to convert integer count of characters into string so that they can be added to the answer string.
                                              
**Link(s) to work**
[run length encoding](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day66.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1482330720995786756)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day66-100daysofcode-freecodecamp-activity-6888092883686068224-w9k7)


### Day 67: January 12, Wednesday
 
**Today's Progress**: Problem : Array Pair Sum Divisibility Problem
                                 Here we are using the technique of remainders so we create a map that keeps frequency of remainders obtained by dividing each element of the array by the given number k.Then in case the remainder is zero and it is odd in frequency, we will return false since then it cannot form pairs.Also the case is same with frequency of k/2 remainder as it requires another number to form pairs.In all other cases any remainder x can be added to the remainder k-x to get divided by the target k so their frequency should match.In case it doesn't we return fale else we return true.
                                              
**Link(s) to work**
[Array Pair Sum Divisibility Problem](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day67.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi/status/1482331553137324032)\
[Post on LinkedIn](https://www.linkedin.com/posts/rakhi-pundhir-97aa0620b_day67-100daysofcode-freeocdecamp-activity-6888093428953960448-x4LT)

### Day 68: January 13, Thursday
 
**Today's Progress**: Problem : Possible captures for rook
                                First find out the location of rook that is the row and column number of the rook's cell then traverse the matrix and check if there is any pawn then increment the counter variable and in case there is any bishop then stop for that iteration and move further till the rook reaches end of the row or column.To check in the upward,downward,right or left direction simply keep row/column common and increment/decrement the other.
                                              
**Link(s) to work**
[Possible captures for rook](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day68.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)


### Day 69: January 14, Friday
 
**Today's Progress**: Problem : Merge arrays without using extra space
                                use pointers technique here and keep on epointer at start of first array and one at start of another array and the thirs one at the end of the first array,now as you traverse the array if element of first array is smaller than the second one then simply move further else swap the values of first and second array but swap the value of second array with the value pointed by the third pointer since it is the largest and so should be sent to the second array.
                                              
**Link(s) to work**
[Merge arrays without using extra space](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day69.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 70: January 15, Saturday
 
**Today's Progress**: Problem : Earliest full bloom
                                 This is based on the fact that we can plant another tree when previous plant is in growing stage so we sort them according to their grow time so that we can plant more trees that time and hence they would require less time to bloom together.Also we add the startdate of previous plant to next one since it was planted after that and then we can take maximum of them.
                                              
**Link(s) to work**
[Earliest full bloom](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day70.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 71: January 16, Sunday
 
**Today's Progress**: Problem : Minimum jumps to reach end of array
                               Here, thake a maxreach to store the maximum index that can be reached from a particular index which is the sum of index and the value at that index.Then also take steps and jump and while traversing the array update them.When you move forward steps are decreased and when the steps becomes zero that means we have completed one jump so increment jumps.When we reach the end of the array then return jump and in case the maxreach becomes lesser than the ith iteration return -1 as it is now not possible to reach the end.
                                              
**Link(s) to work**
[Minimum jumps to reach end of array](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day71.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 72: January 17, Monday
 
**Today's Progress**: Problem : Bellman Ford Algorithm
                                This algorithm is used to find the shortest path from a source node to all other nodes just like Dijkstra's algorithm but Bellman Ford can be used for detecting negative cycles and it works for negative weights also.Assign a status 0 to the sorce node and infinity to all other nodes.Start from the source node and relax its adjacent edges then move to the next node and continue this for n-1 passes where n is the total number of nodes.After n-1 passes we will have the shortest distance.
                                              
**Link(s) to work**
[Bellman Ford Algorithm](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day72.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 73: January 18, Tuesday
 
**Today's Progress**: Problem : Next Permutation
                               Step 1: traverse from right and find the first element that doesn't follow descending order.
                               Step 2:Traverse from right till x and find the smallest number just greater than x
                               Step 3:Swap x and y
                               Step 4:Reverse all from x+1 to end
                               or we can use next_permutation of C++ STL
                                              
**Link(s) to work**
[Next Permutation](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day73.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 74: January 19, Wednesday
 
**Today's Progress**: Problem : Minimum Moves 
                               If target number is even then do some calculations that involve a double and an increment.In case the target number is odd then do some calculations that involve only a double operation.Continue this process till the number od doubles becomes zero or till the target number is greater than one.
                                              
**Link(s) to work**
[Minimum Moves](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day74.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 75: January 20, Thursday
 
**Today's Progress**: Problem : Divide a string into groups of size k
                                We will extract a substring of k characters from the string and keep on pushing that, till complete groups are formed.After the loop, all full groups are included into the answer vector and after this we take remainder to find out how many characters are missing.Append the missing characters to a new string and then fill it by the filler element till the group is completed.
                                              
**Link(s) to work**
[Divide a string into groups of size k](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day75.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 76: January 21, Friday
 
**Today's Progress**: Problem : Rearange array elements by sign
                                We traverse the array and put all negative elements into another array and all positve elements into a third array.Then we again loop over the given array and keep placing the elements into their desired position from the other two arrays using pointers to all the three arrays and we start with placing the first element from the positive element's array.
                                              
**Link(s) to work**
[ Rearange array elements by sign](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day76.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 77: January 22, Saturday
 
**Today's Progress**: Problem : Find all lonely numbers in the array
                                You are given an integer array nums. A number x is lonely when it appears only once, and no adjacent numbers (i.e. x + 1 and x - 1) appear in the array.This problem becomes simple if we try to solve it with the help of maps in C++ STL.We can keep record of the frequency of all array elements and then loop over the array once to check if there exists a number that has come only once int he array and also there is no number present in the array that is its neighbour element and so we increase the count of all such numbers.
                                              
**Link(s) to work**
[Find all lonely numbers in the array](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day77.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 78: January 23, Sunday
 
**Today's Progress**: Problem : Smallest Subarray with sum greater than a given value
                                We keep adding elements till sum becomes greater than x,once it is so we try to decrease length of till sum remains greater than x and keep on comparing the length of this subarray with the minimum length.
                                              
**Link(s) to work**
[Smallest Subarray with sum greater than a given value](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day78.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 79: January 24, Monday
 
**Today's Progress**: Problem : Find minimum operations to make array palindrome
                                We take two pointers start and end since we can merge array elements(adjacent ones only) we check if arr[i] > arr[j] in that case we will merge j and its adjacent value so as to bring the sum closer to arr[i] and same we do for its opposite case.
                                              
**Link(s) to work**
[Find minimum operations to make array palindrome](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day79.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 80: January 25, Tuesday
 
**Today's Progress**: Problem : All Divisions With the Highest Score of a Binary Array
                                It would to efficient if we take two vectors one to store the count of zeroes to the left of an index i and another one to store the count of one's to the right and itself of an index.Then using the sum of respective index find the maximum value and loop over the arrays to find and push those indices into the answer vector for which the sum is equal to the maximum value.
                                              
**Link(s) to work**
[All Divisions With the Highest Score of a Binary Array](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day80.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 81: January 26, Wednesday
 
**Today's Progress**: Problem : Depth First Search in Graph
                                It implements using a stack data structure which works on LIFO principle.In dfs we visit children before siblings of any node.Here, we go into depth of a node and is simply a traversal technique for a graph.
                                              
**Link(s) to work**
[Depth First Search in Graph](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day81.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 82: January 27, Thursday
 
**Today's Progress**: Problem : Detect cycle in an undirected graph using dfs
                                While traversing a node if it happens that the node was already traversed and is also not its parent then there exists a cycle in that graph(undirected) so we make recursive calls when for any unvisited node and pass that node along with its parent.
                                              
**Link(s) to work**
[ Detect cycle in an undirected graph using dfs](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day82.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 83: January 28, Friday
 
**Today's Progress**: Problem : Detect cycle in a directed graph using dfs
                                While traversing the graph if a node is visited then it is not necessary that there exists a cycle as in a directed graph we can reach node from different nodes and to keep check on this we take two visisted arrays one to account for its visit in the current dfs and the other to simply mark it as visisted, cycle exists only when a node is marked visisted in both of these arrays.
                                              
**Link(s) to work**
[ Detect cycle in a directed graph using dfs](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day83.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 84: January 29, Saturday
 
**Today's Progress**: Problem : Number of islands
                                When you find an island increment the count and make recursive calls to check for adjacent cells of the grid, if a cell is land it was included so unmark it and if it is water then do not make any change. 
                                              
**Link(s) to work**
[Number of islands](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day84.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 85: January 30, Sunday
 
**Today's Progress**: Problem : Topological sort using dfs
                                Topological sort is a linear oredering of nodes when a vertex u comes before vertex v for any directed edge from u to v, or we can say that that node comes first in this ordereing that has least indegree.So, we use dfs to store that node in a stack for which function call is over first so that for u to v edge u is always before v.
                                              
**Link(s) to work**
[Topological sort using dfs](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day85.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 86: January 31, Monday
 
**Today's Progress**: Problem : Dijkstra's Algorithm
                                Here, we give an ifinite distance to all nodes and a distance zero to the sorce node and then we take the node with minimum distance and relax its adjacent edges so for this I have used a priority queue that would implement a min heap and store the distance and the node so that we always get a node with least distance.
                                              
**Link(s) to work**
[Dijkstra's Algorithm](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day86.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 87: February 01, Tuesday
 
**Today's Progress**: Problem : Bellman Ford Algorithm
                                This algorithm works for negative edges and can also detect negative edge cycle and here we do exactly n-1 passes and relax every edge of all nodes and incase after n-1 pass there is still a need to relax an edge means there exists a negative cycle.
                                              
**Link(s) to work**
[Bellman Ford Algorithm](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day87.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 88: February 02, Wednesday
 
**Today's Progress**: Problem : Floyd Warshall Algorithm
                                This algorithm is used to find shortest distance between every node if a third node is brought in between them. It fails to work on negative weight cycle but can detect it.
                                              
**Link(s) to work**
[Floyd Warshall Algorithm](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day88.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 89: February 03, Thursday
 
**Today's Progress**: Problem : Disjoint Set Union
                                This is used to find if two nodes belong to the same component or not.Here, we make sets of all nodes and take two arrays parent and rank and when there is a union between two nodes we find their parent using findparent function and then we compare the rank of thier parents.The parent with less rank can be attached to the other and so that becomes its parent node and vice-versa.In case rank of both the parents is same we can make eiehere of them as parent and increase its rank.
                                              
**Link(s) to work**
[Disjoint Set Union](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day89.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 90: February 04, Friday
 
**Today's Progress**: Problem : Krushkal's Alogrithm
                                We have to take the minimum weight edge and insert it into the minimum spanning tree so that no cycle is created in the tree.For this we use disjoint set union.First, we store edges in increasing order of their weights and then take out an edge one by one and check for every edge if the nodes sharing the edge belong to the same component or not because if they do it means that their parent is same so we would no include it.
                                              
**Link(s) to work**
[Krushkal's Algorithm](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day90.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 91: February 05, Saturday
 
**Today's Progress**: Problem : Breadth First Search
                                This is a graph traversal technique and it uses a queue data structure that follows FIFO principle.In bfs we visit siblings before children and insert them into the queue and then pop them one by one and process.
                                              
**Link(s) to work**
[Breadth First Search](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day91.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 92: February 06, Monday
 
**Today's Progress**: Problem : Detect cycle in an undirected graph using bfs
                                while traversing the graph if we encounter a node that is already visited and is also not a parent then it means there exists a cycle so for this we create a queue and store node and its parent in it and traverse the graph using adjacency list.
                                              
**Link(s) to work**
[Detect cycle in an undirected graph using bfs](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day92.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 93: February 07, Tuesday
 
**Today's Progress**: Problem : Detect cycle in a directed graph using bfs
                                We will use topological sort here as it can works only for a directed acyclic graph and so if we are able to find topological ordering for a given directed graph then it is confirm that it does not contain any cycle.
                                              
**Link(s) to work**
[Detect cycle in a directed graph using bfs](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day93.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 94: February 08, Wednesday
 
**Today's Progress**: Problem : Topological Sort using bfs
                                We create an indegree array(no. of incoming egdes to a node) and fill it then push those nodes into a queue for which indegree is zero and also decrease indegree of its adjacent node as in topological ordering for u to v u comes before v that is node with indegree less is before the other. 
                                              
**Link(s) to work**
[Topologicla sort using bfs](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day94.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 95: February 09, Thursday
 
**Today's Progress**: Problem : Prim's Algorithm
                                We take three arrays one for checking if a node is included in the minimum spanning tree or not, one to keep record of the connected edges of included nodes and the last one to maintain parent of a node.Aslo, we use a priority queue(min-heap) to give us the minimum weight edge and its node.
                                              
**Link(s) to work**
[Prim's Algorithm](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day95.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 96: February 10, Friday
 
**Today's Progress**: Problem : Heapify Method
                                First we build a heap and call this method to rearrange the nodes so that they follow heap's property.In max heap the parent is always greare than the child so it checks for this conditiona and if not satisfied it swaps them and continue.
                                              
**Link(s) to work**
[Heapify Method](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day96.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 97: February 11, Saturday
 
**Today's Progress**: Problem : Heap Sort
                                First we build a max heap of the given array elements and then change the first element with the last element and call heapify method to maintain heap's property for the remaining heap and in this process the largest element comes at the last index of the array and so the array starts sorting from the back. 
                                              
**Link(s) to work**
[Heap Sort](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day97.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 98: February 12, Sunday
 
**Today's Progress**: Problem : Bipartite Graph using BFS
                                A bipartite graph is one that can be colored using two different colors such that adjacent nodes have different colors.So, we see that whenever there is a cycle having length odd then the graph cannot be a bipartite else it can be.Here, we have used a queue data structure and bfs traversal to check in the graph if there is any node which has same color as that of its adjacent then we print the graph as not a bipartite one.
                                              
**Link(s) to work**
[Bipartite Graph using BFS](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day98.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 99: February 13, Monday
 
**Today's Progress**: Problem : Bipartite Graph using DFS
                                A bipartite graph is one that can be colored using two different colors such that adjacent nodes have different colors. We make a dfs traversal and start with making the first node of a component of graph as color 1 then check for its adjacent edges.In case the edge is not marked we mark it with the color opposite to its node and make further dfs call and in case the edge has a color we check if that color is same as its adjacent node or not.If it is same we return false.
                                              
**Link(s) to work**
[Bipartite Graph using DFS](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day99.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

### Day 100: February 14, Tuesday
 
**Today's Progress**: Problem : Strongly Connected Components of a Graph using Kosaraju's Algorithm
                                To print all connected components of a graph separately if we perform dfs then all will print together but if we make dfs call in reverse or according to finishing time then we get the desired result.So for this we first find this ordering which is topological ordering and then we take transpose of the graph and then finally call dfs on this transposed graph in order of the nodes obtained from the stack of topological sort.
                                              
**Link(s) to work**
[Strongly Connected Components of a Graph using Kosaraju's Algorithm](https://github.com/Rakhi-Pundhir/100daysofcode/blob/master/day100.cpp)

[Post on twitter](https://twitter.com/pundhir_rakhi)\
[Post on LinkedIn](https://www.linkedin.com/in/rakhi-pundhir-97aa0620b/)

             
