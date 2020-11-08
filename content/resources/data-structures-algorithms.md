+++
title = "Data Structures and Algorithms"
date = 2020-11-08
[taxonomies]
tags = ["data-structures", "algorithms", "interviews"]
+++

Many times in interviews for a data science/ tech role, you will have to answer programming (data structures and algorithms) questions. The reason is that algorithms/data structures commonly occur in programming, and they test the ability to *think computationally* and solve problems using programming - knowledge of data science/stats/maths is good but in addition you need to be able to *program*.

# Theory

## Books

**These are books SPECIFICALLY for algos/data structures training for interviews**

Cracking the Coding Interview:  [https://www.amazon.co.uk/Cracking-Coding-Interview-6th-Programming/dp/0984782850/](https://www.amazon.co.uk/Cracking-Coding-Interview-6th-Programming/dp/0984782850/)

Elements of Programming Interviews: 

**These are textbooks for a standard Data Structures and Algorithms course (e.g. MA314)**

Introduction to Algorithms (commonly referred to as the "CLRS" book): [https://www.amazon.co.uk/Introduction-Algorithms-Thomas-H-Cormen/dp/0262033844/](https://www.amazon.co.uk/Introduction-Algorithms-Thomas-H-Cormen/dp/0262033844/)

Grokking Algorithms: [https://www.amazon.co.uk/Grokking-Algorithms-illustrated-programmers-curious/dp/1617292230/](https://www.amazon.co.uk/Grokking-Algorithms-illustrated-programmers-curious/dp/1617292230/)

Algorithms: [https://www.amazon.co.uk/Algorithms-Robert-Sedgewick/dp/032157351X/](https://www.amazon.co.uk/Algorithms-Robert-Sedgewick/dp/032157351X/)

Steven Skiena [https://www.amazon.co.uk/gp/product/0387948600/](https://www.amazon.co.uk/gp/product/0387948600/)

**These are geared towards competitive programming, but are quite relevant and useful**

Competitive Programming 3 : [https://www.amazon.com/Competitive-Programming-3rd-Steven-Halim/dp/B00FG8MNN8](https://www.amazon.com/Competitive-Programming-3rd-Steven-Halim/dp/B00FG8MNN8)

Guide to Competitive Programming : [https://www.amazon.co.uk/Guide-Competitive-Programming-Algorithms-Undergraduate/dp/3030393569/](https://www.amazon.co.uk/Guide-Competitive-Programming-Algorithms-Undergraduate/dp/3030393569/)

### Data Structures to Know:
+ Arrays
+ Linked Lists, Stacks, Queues
+ Tree (Tree, Binary Tree, Binary Search Tree, Redß-Black Tree, etc.)
+ Heap 
+ Hash Table
+ Trie
+ Graphs (both directed and undirected)

### Algorithms to Know

+ Sorting: Bubble Sort, Merge Sort, Quick Sort, Radix/Bucket Sort, Heapsort

+ Graph Traversals: Depth First Search, Breadth First Search


## Exercises

The only way to get better is to expose yourself to more exercises. There are tons of platforms (Leetcode, Hackerrank), and competitions available to do so

Going through https://www.teamblind.com/post/New-Year-Gift---Curated-List-of-Top-75-LeetCode-Questions-to-Save-Your-Time-OaM1orEU or Project Euler https://projecteuler.net/ could be a good start


<!-- 1. Two Sum (Easy)
+ https://leetcode.com/problems/two-sum/
+ Find the two indices such that the values sum to target
+ O(n^2). Loop through until you find it
+ Could it be improved by sorting?
+ From the solution there is a O(n) way to do this
+ Use a hash table
+ For every element, check if it's complement is in the table


121. Best Time to Buy and Sell Stock. (Easy)
+ https://leetcode.com/problems/best-time-to-buy-and-sell-stock/submissions/
+ Need to find the greatest difference between array[right] - array[left], left < right
+ O(n). Loop through, set left to be the current global minima and set best to the greatest difference.


122. Best Time to Buy and Sell Stock II (Easy)
+ https://leetcode.com/problems/best-time-to-buy-and-sell-stock-ii/
+ Same as 121, but you can do any number of trades
+ O(n). Loop through, if the difference between prices[i] - prices[i - 1] is positive add it to the running sum.

217. Contains Duplicate (Easy)
+ https://leetcode.com/problems/best-time-to-buy-and-sell-stock/submissions/
+ Return true if there are duplicates of any value in the array
+ O(n). Use a (hash)map

238. Product of Array Except Self (Medium)
+ https://leetcode.com/problems/product-of-array-except-self/
+ Create a solution array, where every solution[j] is the product of all original array values except for array[j]
+ Had to look at the solution for this
+ O(n) time, O(1) space. 
+ Create the solution array and loop through left to right. 
+ For each index, set answer[i] to be the running product of the entries to the left of it
+ Loop through right to left, keeping track of the running product from right to left.
+ Multiply solution[j] by the running product from right to left

53. Maximum Subarray (Easy)
+ https://leetcode.com/problems/maximum-subarray/
+ Find the largest subarray sum
+ Had to refer to the Laarksonen book
+ O(n) time
+ loop through the array. If the current running sum > 0, add  num[i]. Otherwise set the current running sum to num[i]
+ Keep track of the best subarray sum with best = max(best, sum)

153. Find Minimum in Rotated Sorted Array (Medium)
+ https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/
+ A sorted array is rotated
+ O(n) time
+ loop through the array. Since it is sorted, if num[i - 1] > num[i] then num[i] is the smallest value
+ Is there a O(log(n)) way to do this?
+ Yes from the solution using binary search


33. Search in Rotated Sorted Array
+ https://leetcode.com/problems/3sum/
+ A sorted array is rotated, find a given value, or -1 if it is not present
+ O(log(n)) time.
+ Modify the solution to 153; B-search to find the lowest index. 
+ Then do a B-search on the filtered array i.e. arr[min...n - 1] or arr[1.. min]

33. Search in Rotated Sorted Array
+ https://leetcode.com/problems/3sum/
+ A sorted array is rotated, find a given value, or -1 if it is not present
+ O(log(n)) time.
+ Modify the solution to 153; B-search to find the lowest index. 
+ Then do a B-search on the filtered array i.e. arr[min...n - 1] or arr[1.. min]

15. 3Sum (Medium)
+ https://leetcode.com/problems/3sum/
+ Find all triples that sum to 0
+ O(n^2) time
+ Had to look this up. Sort the array. Loop through for each i. For each i,  set two pointers l, r. if sum = nums[i] + nums[l] + nums[r] ==  target then add to the set
+ if sum < target then we need to increase l ; if sum > target we need to decrease r;

11. Container With Most Water (Medium)

+ https://leetcode.com/problems/container-with-most-water/
+ Find the two indices such that (height[i] - height[j]) * (j - i) is maximised
+ Had to look this up
+ O(n). The best container must be contained within [0, n]. 

371. Sum of Two Integers (Medium)
+ https://leetcode.com/problems/sum-of-two-integers/
+ Had to look this up; Sum up two integers only using bit operations
+ O(1) time
+ Full adder logic; Recursively Add XOR representation +  shifted Carry (AND)

191. Number of 1 Bits (Easy)
+ https://leetcode.com/problems/number-of-1-bits/
+ Easy. Increment count with (n & 1) and bitshift n, n >>=  1 until n =0 

268. Missing Number (Easy)
+ https://leetcode.com/problems/missing-number/ 
+ O(n) time, My solution used the difference between (n + 1)(n) / 2
+ There's probably a way to it using bitsets (From Solution, yes and that is to use XOR, which is a self-inverse.)

190. Reverse Bits (Easy)
+ https://leetcode.com/problems/reverse-bits/
+ O(1) time, simple, reverse the bits
+ Very elegant solution in the solutions: using bitmasks and magic number-of-1-bits

70. Climbing Stairs (Easy)
+ https://leetcode.com/problems/climbing-stairs/
+ O(n) time , O(n) space. Standard dynamic programming
+ Count the number of ways you can sum any number of 1s, 2s to a given number

322. Coin Change (Medium)
+ https://leetcode.com/problems/climbing-stairs/
+ O(n) time , O(n) space. Standard dynamic programming
+ Same as 70 except count the number of ways you can sum any number of a set of numbers.

300. Longest Increasing Subsequence
+ https://leetcode.com/problems/longest-increasing-subsequence/
+ Looked it up in the Laarksonen book.	
+ O(n^2 ) complexity, loop through, use memoisation to cache.
+ the solution has a solution that uses binary search for O(nlog(n)) complexity

62. Unique Paths (Medium)
+ https://leetcode.com/problems/unique-paths/
+ Paths in a grid if you can only move right and down
+ Easy (Comabinatorics, ) (m + n - 2)C(n - 1), however you need to use Dynamic Programming to calculate the binomial coefficient
+ O(nm) space complexity, O(nm) time complexity

377. Combination Sum IV (Medium)
https://leetcode.com/problems/combination-sum-iv/
+ Essentially the same as 322, standard dynamic programming, O(m) space, O(nm) time
+ Had to use Java as there is overflow using C++

378. Jump Game 
https://leetcode.com/problems/jump-game/
+ For each index i, you can jump at most array[i], and you have to find out if array[n-1] is reachable
+ Traverse the array from the right to left, and see if there is a path from the origin 0
+ O(n) time;

91. Decode Ways
+ https://leetcode.com/problems/decode-ways/
+ How many ways can a string of digits be decoded if 1 -> A, 2-> B...
+ Looked this up a bit
+ Standard Dynamic Programming: every message can be decoded as e.g. (a1 a2) (a3), (a2) (a3) if they are valid
+ O(n) space, O(n) time.	

198. House Robber (Easy)
+ https://leetcode.com/problems/house-robber/submissions/
+ What's the greatest sum by a subset of indices where no indices are adjacent
+ Standard Dynamic Programming. Loop through, at each index, consider whether the best sum for the adjacent cache[i -1] is better cache[i - 2] + nums[i]
+ O(n) space, O(n) time.

213. House Robber II (Medium)
+ https://leetcode.com/problems/house-robber-ii/
+ Same as 198, What's the greatest sum by a subset of indices where no indices are adjacent. However the houses are in the circle, i.e. you cannot have both 0 and n - 1
+ O(n) space. Use two arrays to keep track, one from 1.. n - 1, one from 0... n -2. Then the solution is in the maximum of these two

139. Word Break (Medium)
+ https://leetcode.com/problems/word-break/
+ Can a string be covered down by a set of substrings

141. Linked List Cycle (Easy)
+ https://leetcode.com/problems/linked-list-cycle/submissions/
+ Detect a cycle in a Linked List
+ Tortoise and Hare pointers method; Have a pointer iterate two steps, one pointer iterate one step. If they coincide, then there is a cycle

73. Set Matrix Zeroes (Medium)
+ https://leetcode.com/problems/set-matrix-zeroes/submissions/
+ If an entry is 0, set its row and column  to 0s
+ O(m + n) space complexity solution; Keep track of the columns and rows to set to 0. Then loop through for O(mn) time complexity.
+ There is a O(1) space complexity solution, from the solution it is to use the matrix entries as flags.

54. Spiral Matrix (Medium)
+ https://leetcode.com/problems/spiral-matrix/
+ Ad hoc solution, same as Project Euler

48. Rotate Image (Medium)
+ https://leetcode.com/problems/rotate-image/
+ Rotate the entries of a matrix, ad hoc solution -->




