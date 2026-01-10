## Title
Garden Planting

## Slug
garden-planting

## Difficulty
Medium

## Description
A gardener plants flowers in pots 1 to n. The garden looks 'complete' from the entrance if pots 1 to k all have flowers.

There is a sequence of $n$ pots indexed from $1$ to $n$. Initially, all pots are **empty**.

You plant in the pots one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you plant in the pot at the position `sequence[i-1]`.

A state is called **complete** if, after performing $k$ steps, exactly the first $k$ pots (indices $1$ to $k$) are planted and all other pots are empty.

Your task is to calculate how many times the system becomes **complete** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "__Y__" (Not complete)
- Step 2 (index 2): "_YY__" (Not complete)
- Step 3 (index 4): "_YYY_" (Not complete)
- Step 4 (index 1): "YYYY_" (complete: first 4 are planted)
- Step 5 (index 5): "YYYYY" (complete: first 5 are planted)
Total complete states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "___Y" (Not complete)
- Step 2 (index 1): "Y__Y" (Not complete)
- Step 3 (index 2): "YY_Y" (Not complete)
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
