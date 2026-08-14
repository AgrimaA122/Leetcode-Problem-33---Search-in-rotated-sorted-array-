# Leetcode-Problem-33---Search-in-rotated-sorted-array-
Leetcode solution for problem number 33

### Description

In this experiment, the **Search in Rotated Sorted Array** problem was solved using a modified **Binary Search** algorithm. The sorted array is rotated at some point, so at every step we identify which half of the array is sorted and check whether the target lies within that half.

### Algorithm

1. Take the rotated sorted array and target as input.
2. Set `start` to the first index and `end` to the last index.
3. Calculate the middle index using `mid = start + (end - start) / 2`.
4. Check if `nums[mid]` is equal to the target.
5. Determine which half of the array is sorted.
6. Check whether the target lies within the sorted half.
7. If it does, search that half; otherwise, search the other half.
8. Repeat until the target is found or `start > end`.
9. Return the target's index, or `-1` if it is not found.

### Time Complexity

**O(log n)** — The search space is divided approximately in half during every iteration.

### Space Complexity

**O(1)** — Only a few variables such as `start`, `end`, and `mid` are used.
