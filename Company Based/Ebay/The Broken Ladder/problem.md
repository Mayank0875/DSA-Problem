## Title

The Broken Ladder

## Slug

the-broken-ladder

## Difficulty

Medium

## Description

An adventurer is attempting to scale a high tower, but the ancient ladder has fallen apart. He finds a pile of scattered rungs on the ground, each marked with a unique height integer. To safely climb a section of the tower, he needs to construct a sequence of rungs that correspond to consecutive integers (e.g., `4, 5, 6, 7`).

The adventurer can start building his ladder from any rung number, but he wants to build the longest possible continuous section to maximize his climb.

Given an unsorted array of integers `rungs` representing the height values of the available pieces, return the length of the longest consecutive sequence of rungs that can be assembled.

You must write an algorithm that runs in $O(n)$ time.

## Examples

### 1

#### Input

6 
100 4 200 1 3 2

#### Output

4

#### Explanation

The longest consecutive elements sequence is `[1, 2, 3, 4]`. Therefore its length is 4.
    
### 2

#### Input

10 
0 3 7 2 5 8 4 6 0 1

#### Output

9

#### Explanation

The consecutive sequence is `[0, 1, 2, 3, 4, 5, 6, 7, 8]`. Note that `0` appears twice, but sets handle uniqueness.
  

## Input Format  

- The first line contains an integer `n`, the number of rungs.
- The second line contains `n` space-separated integers representing the `rungs` array.

## Output Format  

- Return a single integer representing the length of the longest consecutive sequence.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- -1e9 ≤ rungs[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, hash-table

## Company
ebay