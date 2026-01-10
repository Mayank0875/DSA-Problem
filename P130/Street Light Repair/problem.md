## Title
Street Light Repair

## Slug
street-light-repair

## Difficulty
Medium

## Description
Electricians fix broken streetlights. The street is 'safely lit' from the start if lights 1 to k are all fixed.

There is a sequence of $n$ lights indexed from $1$ to $n$. Initially, all lights are **broken**.

You repair the lights one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you repair the light at the position `sequence[i-1]`.

A state is called **safely lit** if, after performing $k$ steps, exactly the first $k$ lights (indices $1$ to $k$) are fixed and all other lights are broken.

Your task is to calculate how many times the system becomes **safely lit** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "xxoxx" (Not safely lit)
- Step 2 (index 2): "xooxx" (Not safely lit)
- Step 3 (index 4): "xooox" (Not safely lit)
- Step 4 (index 1): "oooox" (safely lit: first 4 are fixed)
- Step 5 (index 5): "ooooo" (safely lit: first 5 are fixed)
Total safely lit states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "xxxo" (Not safely lit)
- Step 2 (index 1): "oxxo" (Not safely lit)
- Step 3 (index 2): "ooxo" (Not safely lit)
- Step 4 (index 3): "oooo" (safely lit)
Total safely lit states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was safely lit.

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
