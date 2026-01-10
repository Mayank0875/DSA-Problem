## Title
Security Checkpoints

## Slug
security-checkpoints

## Difficulty
Medium

## Description
Guards man checkpoints 1 to n. The perimeter is 'secured' up to point k if all checkpoints 1 to k are manned.

There is a sequence of $n$ checkpoints indexed from $1$ to $n$. Initially, all checkpoints are **unmanned**.

You staff the checkpoints one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you staff the checkpoint at the position `sequence[i-1]`.

A state is called **secured** if, after performing $k$ steps, exactly the first $k$ checkpoints (indices $1$ to $k$) are manned and all other checkpoints are unmanned.

Your task is to calculate how many times the system becomes **secured** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not secured)
- Step 2 (index 2): "01100" (Not secured)
- Step 3 (index 4): "01110" (Not secured)
- Step 4 (index 1): "11110" (secured: first 4 are manned)
- Step 5 (index 5): "11111" (secured: first 5 are manned)
Total secured states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not secured)
- Step 2 (index 1): "1001" (Not secured)
- Step 3 (index 2): "1101" (Not secured)
- Step 4 (index 3): "1111" (secured)
Total secured states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was secured.

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
