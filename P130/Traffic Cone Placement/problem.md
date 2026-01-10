## Title
Traffic Cone Placement

## Slug
traffic-cone-placement

## Difficulty
Medium

## Description
Cones are placed on marks 1 to n. The lane is 'closed' if marks 1 to k have cones.

There is a sequence of $n$ marks indexed from $1$ to $n$. Initially, all marks are **open**.

You block the marks one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you block the mark at the position `sequence[i-1]`.

A state is called **closed** if, after performing $k$ steps, exactly the first $k$ marks (indices $1$ to $k$) are blocked and all other marks are open.

Your task is to calculate how many times the system becomes **closed** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "__^__" (Not closed)
- Step 2 (index 2): "_^^__" (Not closed)
- Step 3 (index 4): "_^^^_" (Not closed)
- Step 4 (index 1): "^^^^_" (closed: first 4 are blocked)
- Step 5 (index 5): "^^^^^" (closed: first 5 are blocked)
Total closed states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "___^" (Not closed)
- Step 2 (index 1): "^__^" (Not closed)
- Step 3 (index 2): "^^_^" (Not closed)
- Step 4 (index 3): "^^^^" (closed)
Total closed states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was closed.

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
