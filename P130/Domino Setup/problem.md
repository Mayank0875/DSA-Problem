## Title
Domino Setup

## Slug
domino-setup

## Difficulty
Medium

## Description
You are standing up dominoes in a line. The line is 'contiguous' if dominoes 1 through k are all standing.

There is a sequence of $n$ dominoes indexed from $1$ to $n$. Initially, all dominoes are **down**.

You stand up the dominoes one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you stand up the domino at the position `sequence[i-1]`.

A state is called **contiguous** if, after performing $k$ steps, exactly the first $k$ dominoes (indices $1$ to $k$) are standing and all other dominoes are down.

Your task is to calculate how many times the system becomes **contiguous** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "__|__" (Not contiguous)
- Step 2 (index 2): "_||__" (Not contiguous)
- Step 3 (index 4): "_|||_" (Not contiguous)
- Step 4 (index 1): "||||_" (contiguous: first 4 are standing)
- Step 5 (index 5): "|||||" (contiguous: first 5 are standing)
Total contiguous states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "___|" (Not contiguous)
- Step 2 (index 1): "|__|" (Not contiguous)
- Step 3 (index 2): "||_|" (Not contiguous)
- Step 4 (index 3): "||||" (contiguous)
Total contiguous states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was contiguous.

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
