## Title
Mountain Heights

## Slug
mountain-heights

## Difficulty
Easy

## Description
A geographer lists the elevation of peaks in a mountain range.

The satellite data records the elevation of $N$ mountains in an array. To classify peaks, the mapper needs to assign a rank to every mountain based on its elevation.

The ranking rules are simple: the mountain with the **smallest** elevation gets **Rank 1**. The next distinct elevation gets **Rank 2**, and so on.

If two or more mountains have the exact same elevation, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each mountain's elevation with its corresponding rank.

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
All mountains share the same elevation, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of mountains.
- The second line contains `n` space-separated integers representing the elevations.

## Output Format
- Return an array of integers where each element is the rank of the corresponding mountain.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
