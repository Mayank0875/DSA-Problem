## Title
City Skyline Building

## Slug
city-skyline-building

## Difficulty
Medium

## Description
Skyscrapers are topped out. The skyline is 'complete' from the west if buildings 1 to k are finished.

There is a sequence of $n$ buildings indexed from $1$ to $n$. Initially, all buildings are **in-progress**.

You complete the buildings one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you complete the building at the position `sequence[i-1]`.

A state is called **complete** if, after performing $k$ steps, exactly the first $k$ buildings (indices $1$ to $k$) are finished and all other buildings are in-progress.

Your task is to calculate how many times the system becomes **complete** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "nnYnn" (Not complete)
- Step 2 (index 2): "nYYnn" (Not complete)
- Step 3 (index 4): "nYYYn" (Not complete)
- Step 4 (index 1): "YYYYn" (complete: first 4 are finished)
- Step 5 (index 5): "YYYYY" (complete: first 5 are finished)
Total complete states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "nnnY" (Not complete)
- Step 2 (index 1): "YnnY" (Not complete)
- Step 3 (index 2): "YYnY" (Not complete)
- Step 4 (index 3): "YYYY" (complete)
Total complete states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was complete.

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
