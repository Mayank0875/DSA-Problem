## Title

Raju's Kite Festival

## Slug

rajus-kite-festival

## Difficulty

Easy

## Description

Raju is organizing a grand Patang (kite) festival in his village. He records the flying heights of $N$ kites in an array. To declare the results, he needs to assign a rank to every kite based on its height.

The ranking rules are simple: the kite at the lowest height gets Rank 1. The next distinct height gets Rank 2, and so on. If two or more kites are flying at the exact same height, they must receive the same rank. The ranks must be integers starting from 1. Your task is to help Raju replace each kite's height with its corresponding rank.

## Examples

### 1

#### Input

4
40 10 20 30

#### Output

4 1 2 3

#### Explanation

10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).
    
### 2

#### Input

3
2 2 2

#### Output

1 1 1

#### Explanation

All kites are at the same height, so they share Rank 1.

## Input Format  

- The only input line has an integer n.
- The Second line contains the array/list of integers `arr` representing kite heights.


## Output Format  

- Return an array/list of integers where each element is the rank of the corresponding kite height.
  

## Constraints  

- 1 ≤ arr.length ≤ 1e5
- -1e9 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, hash-table

## Company
facebook