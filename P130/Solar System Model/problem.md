## Title
Solar System Model

## Slug
solar-system-model

## Difficulty
Medium

## Description
Planets are placed in orbits 1 to n. The model is 'accurate' out to orbit k if planets 1 to k are placed.

There is a sequence of $n$ orbits indexed from $1$ to $n$. Initially, all orbits are **empty**.

You populate the orbits one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you populate the orbit at the position `sequence[i-1]`.

A state is called **accurate** if, after performing $k$ steps, exactly the first $k$ orbits (indices $1$ to $k$) are occupied and all other orbits are empty.

Your task is to calculate how many times the system becomes **accurate** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "ooOoo" (Not accurate)
- Step 2 (index 2): "oOOoo" (Not accurate)
- Step 3 (index 4): "oOOOo" (Not accurate)
- Step 4 (index 1): "OOOOo" (accurate: first 4 are occupied)
- Step 5 (index 5): "OOOOO" (accurate: first 5 are occupied)
Total accurate states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "oooO" (Not accurate)
- Step 2 (index 1): "OooO" (Not accurate)
- Step 3 (index 2): "OOoO" (Not accurate)
- Step 4 (index 3): "OOOO" (accurate)
Total accurate states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was accurate.

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
