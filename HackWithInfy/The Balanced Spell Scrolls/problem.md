## Title

The Balanced Spell Scrolls

## Slug

the-balanced-spell-scrolls

## Difficulty

Hard

## Description

n the Archives of Arcana, a young wizard named Elara is organizing a long sequence of spell scrolls. Each scroll has a specific non-negative power level, represented by an integer in an array a of length n.

A sequence of scrolls (a continuous subarray) is considered balanced if the total power of the scrolls is equal to the “missing essence” of that sequence.

The missing essence is defined as the MEX (Minimum Excluded Value) of the power levels in the subarray.

The MEX of a set of numbers is the smallest non-negative integer that does not appear in the set.
For example:

MEX of [1, 2] is 0
MEX of [0, 2] is 1
MEX of [0, 1, 2] is 3

Your task is to count the number of non-empty continuous subarrays for which the sum of the elements is exactly equal to the MEX of the elements.

## Examples

### 1

#### Input

5
0 1 2 0 1

#### Output

4

#### Explanation

The balanced subarrays are:
- `[0, 1, 2]` (Indices 0-2): Sum = 3, MEX = 3.
- `[1, 2, 0]` (Indices 1-3): Sum = 3, MEX = 3.
- `[2, 0, 1]` (Indices 2-4): Sum = 3, MEX = 3.
- `[0, 1, 2, 0]` (Indices 0-3): Sum = 3, MEX = 3.
    
### 2

#### Input

3
1 1 1

#### Output

0

#### Explanation

No subarray satisfies the condition. For `[1]`, Sum=1, MEX=0. For `[1, 1]`, Sum=2, MEX=0.
  

## Input Format  

- The first line contains a single integer $n$ — the length of the array.
- The second line contains $n$ space-separated integers a_1, a_2, ...., a_n.

## Output Format  

- Return single integer representing the number of balanced subarrays.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ a_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, maths, dynamic-programming, two-pointers, hackwithinfy

## Companies
infosys