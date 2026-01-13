## Title
Sound Levels

## Slug
sound-levels

## Difficulty
Easy

## Description
An audio engineer checks the volume of different tracks.

The mixing board records the decibel level of $N$ tracks in an array. To balance the mix, the engineer needs to assign a rank to every track based on its decibel level.

The ranking rules are simple: the track with the **smallest** decibel level gets **Rank 1**. The next distinct decibel level gets **Rank 2**, and so on.

If two or more tracks have the exact same decibel level, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each track's decibel level with its corresponding rank.

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
All tracks share the same decibel level, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of tracks.
- The second line contains `n` space-separated integers representing the decibel levels.

## Output Format
- Return an array of integers where each element is the rank of the corresponding track.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
