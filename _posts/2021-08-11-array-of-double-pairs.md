---
layout: post
title: "Array of Doubled Pairs"
date: 2021-08-11
---
This is how I approached the following problem using UMPIRE method

# Problem statement 

Given an array of integers _arr_ of even length, return true if and only if it is possible to reorder it such that _arr[2 * i + 1] = 2 * arr[2 * i]_ for every _0 <= i <= len(arr)/2_ 

# Understand

Input: arr = [1] or arr = [1,2,3] or arr = [1,2,3,4,5] -> won't be the case 

Input: arr = []
Output: true

Input: arr = [1,1]\
output: false

Input: arr = [3,1,3,6]\
output: false

Input: arr = [2,1,2,6]\
Output: false

Input: arr = [1,2,4,16,8,4]\
Output: false

Input: arr = [1,2]\
Output: true\
Explanation: [1,2] satisfies the given condition

Input: arr = [4,-2,2,-4]\
Output: true\
Explanation: We can take two groups, [-2,-4] and [2,4] to form [-2,-4,2,4] or [2,4,-2,-4]

# Match

**List**
```sh
// iterate though arr with i
    if arr[2 * i + 1] != 2 * arr[2 * i]:
        return False
return True
```
