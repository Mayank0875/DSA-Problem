## Title

Lone Magic Stone

## Slug

lone-magic-stone

## Difficulty

Medium

## Description

An apprentice mage is sorting a collection of magic arr. The arr are arranged in a line, sorted by their magical energy value. Every type of stone should appear exactly twice, side-by-side, except for one special stone that appears only once.
The apprentice needs your help to quickly find the energy value of this unique, lone stone. Given the sorted sequence of stone energy values, write an efficient function to return the value of the single stone that appears only once.


You must write an algorithm with O(log n) runtime complexity

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of arr.
- The second line contains n space-separated integers representing the sorted energy values of the arr.

## Output Format

- Return a single integer: the energy value of the stone that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array
