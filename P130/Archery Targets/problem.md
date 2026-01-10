## Title
Archery Targets

## Slug
archery-targets

## Difficulty
Medium

## Description
Targets 1 to n are hit. A 'perfect streak' exists if targets 1 to k are all hit.

There is a sequence of $n$ targets indexed from $1$ to $n$. Initially, all targets are **standing**.

You hit the targets one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you hit the target at the position `sequence[i-1]`.

A state is called **streak** if, after performing $k$ steps, exactly the first $k$ targets (indices $1$ to $k$) are hit and all other targets are standing.

Your task is to calculate how many times the system becomes **streak** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "OOXOO" (Not streak)
- Step 2 (index 2): "OXXOO" (Not streak)
- Step 3 (index 4): "OXXXO" (Not streak)
- Step 4 (index 1): "XXXXO" (streak: first 4 are hit)
- Step 5 (index 5): "XXXXX" (streak: first 5 are hit)
Total streak states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "OOOX" (Not streak)
- Step 2 (index 1): "XOOX" (Not streak)
- Step 3 (index 2): "XXOX" (Not streak)
- Step 4 (index 3): "XXXX" (streak)
Total streak states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was streak.

## Constraints
- 1 ≤ n ≤ 10^4
- `sequence` is a permutation of numbers from $1$ to $n$.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy

## Company
google
