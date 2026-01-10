## Title
Bridge Construction

## Slug
bridge-construction

## Difficulty
Medium

## Description
Engineers are building a bridge segment by segment. The bridge is 'walkable' up to point k only if all segments 1 to k are built.

There is a sequence of $n$ segments indexed from $1$ to $n$. Initially, all segments are **missing**.

You construct the segments one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you construct the segment at the position `sequence[i-1]`.

A state is called **walkable** if, after performing $k$ steps, exactly the first $k$ segments (indices $1$ to $k$) are built and all other segments are missing.

Your task is to calculate how many times the system becomes **walkable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "__=__" (Not walkable)
- Step 2 (index 2): "_==__" (Not walkable)
- Step 3 (index 4): "_===_" (Not walkable)
- Step 4 (index 1): "====_" (walkable: first 4 are built)
- Step 5 (index 5): "=====" (walkable: first 5 are built)
Total walkable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "___=" (Not walkable)
- Step 2 (index 1): "=__=" (Not walkable)
- Step 3 (index 2): "==_=" (Not walkable)
- Step 4 (index 3): "====" (walkable)
Total walkable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was walkable.

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
