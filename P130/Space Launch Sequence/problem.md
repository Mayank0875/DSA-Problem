## Title
Space Launch Sequence

## Slug
space-launch-sequence

## Difficulty
Medium

## Description
Systems 1 to n are checked. The rocket is 'GO' for launch level k if systems 1 to k are green.

There is a sequence of $n$ systems indexed from $1$ to $n$. Initially, all systems are **red**.

You verify the systems one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you verify the system at the position `sequence[i-1]`.

A state is called **GO** if, after performing $k$ steps, exactly the first $k$ systems (indices $1$ to $k$) are green and all other systems are red.

Your task is to calculate how many times the system becomes **GO** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "RRGRR" (Not GO)
- Step 2 (index 2): "RGGRR" (Not GO)
- Step 3 (index 4): "RGGGR" (Not GO)
- Step 4 (index 1): "GGGGR" (GO: first 4 are green)
- Step 5 (index 5): "GGGGG" (GO: first 5 are green)
Total GO states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "RRRG" (Not GO)
- Step 2 (index 1): "GRRG" (Not GO)
- Step 3 (index 2): "GGRG" (Not GO)
- Step 4 (index 3): "GGGG" (GO)
Total GO states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was GO.

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
