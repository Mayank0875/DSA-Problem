## Title
Cryptocurrency Blockchain

## Slug
cryptocurrency-blockchain

## Difficulty
Medium

## Description
Blocks are validated. The chain is 'verified' up to height k if blocks 1 to k are all valid.

There is a sequence of $n$ blocks indexed from $1$ to $n$. Initially, all blocks are **pending**.

You validate the blocks one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you validate the block at the position `sequence[i-1]`.

A state is called **verified** if, after performing $k$ steps, exactly the first $k$ blocks (indices $1$ to $k$) are valid and all other blocks are pending.

Your task is to calculate how many times the system becomes **verified** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "??V??" (Not verified)
- Step 2 (index 2): "?VV??" (Not verified)
- Step 3 (index 4): "?VVV?" (Not verified)
- Step 4 (index 1): "VVVV?" (verified: first 4 are valid)
- Step 5 (index 5): "VVVVV" (verified: first 5 are valid)
Total verified states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "???V" (Not verified)
- Step 2 (index 1): "V??V" (Not verified)
- Step 3 (index 2): "VV?V" (Not verified)
- Step 4 (index 3): "VVVV" (verified)
Total verified states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was verified.

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
