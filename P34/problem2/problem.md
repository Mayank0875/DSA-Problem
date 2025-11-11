## Title

The Phantom Cipher

## Slug

phantom-cipher

## Difficulty

Medium

## Description

A hacker must decode an encrypted sequence where one value hides without a pair. The sequence is generated from the first n^2 terms of the multiplication table, but one element is missing. Your task is to find the missing value.

For example, the 3 * 3 multiplication table is as follows:
    [[1, 2, 3], [2, 4, 6], [3, 6, 9]]

The numbers in increasing order are [1,2,2,3,3,4,6,6,9], but one element is missing. The hacker knows the sequence should have 9 elements, but only 8 are provided. The missing value is the one that would be the median when the sequence is sorted.

For n=3, the full sorted sequence is [1,2,2,3,3,4,6,6,9], and the median (the middle value) is 3. But if one value is missing, the hacker must deduce which one is missing.

In this problem, you are to find the median of the sorted list of n*n numbers from the multiplication table, assuming one value is missing. But note: the problem is actually to compute the median for the complete set, and the input is just n.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The numbers in increasing order are [1,2,2,3,3,4,6,6,9], so the median (the 5th element in 1-indexing) is 3.
    
### 2

#### Input

5

#### Output

8

#### Explanation
For n=5, the sorted list has 25 elements. The median is the 13th element (since (25+1)/2=13). The value is 8.
  

## Input Format  

- The only input line has an integer n.

## Output Format  

- Return one integer: the answer to the problem.
  

## Constraints  

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory<｜begin▁of▁sentence｜>