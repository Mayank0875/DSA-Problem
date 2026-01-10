## Title
Museum Exhibit Setup

## Slug
museum-exhibit-setup

## Difficulty
Medium

## Description
Artifacts are placed in cases 1 to n. The wing is 'ready' if cases 1 to k are filled.

There is a sequence of $n$ cases indexed from $1$ to $n$. Initially, all cases are **empty**.

You fill the cases one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you fill the case at the position `sequence[i-1]`.

A state is called **ready** if, after performing $k$ steps, exactly the first $k$ cases (indices $1$ to $k$) are filled and all other cases are empty.

Your task is to calculate how many times the system becomes **ready** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not ready)
- Step 2 (index 2): "01100" (Not ready)
- Step 3 (index 4): "01110" (Not ready)
- Step 4 (index 1): "11110" (ready: first 4 are filled)
- Step 5 (index 5): "11111" (ready: first 5 are filled)
Total ready states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not ready)
- Step 2 (index 1): "1001" (Not ready)
- Step 3 (index 2): "1101" (Not ready)
- Step 4 (index 3): "1111" (ready)
Total ready states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was ready.

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
