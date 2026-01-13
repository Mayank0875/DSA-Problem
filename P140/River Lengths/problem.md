## Title
River Lengths

## Slug
river-lengths

## Difficulty
Easy

## Description
A geography student compares the lengths of major rivers.

The atlas records the length (km) of $N$ rivers in an array. To complete the report, the student needs to assign a rank to every river based on its length (km).

The ranking rules are simple: the river with the **smallest** length (km) gets **Rank 1**. The next distinct length (km) gets **Rank 2**, and so on.

If two or more rivers have the exact same length (km), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each river's length (km) with its corresponding rank.

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
All rivers share the same length (km), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of rivers.
- The second line contains `n` space-separated integers representing the length (km)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding river.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
