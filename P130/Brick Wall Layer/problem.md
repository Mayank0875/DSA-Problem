## Title
Brick Wall Layer

## Slug
brick-wall-layer

## Difficulty
Medium

## Description
A mason places bricks in a row. The wall is 'solid' from the left corner if bricks 1 to k are all placed.

There is a sequence of $n$ bricks indexed from $1$ to $n$. Initially, all bricks are **missing**.

You place the bricks one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you place the brick at the position `sequence[i-1]`.

A state is called **solid** if, after performing $k$ steps, exactly the first $k$ bricks (indices $1$ to $k$) are placed and all other bricks are missing.

Your task is to calculate how many times the system becomes **solid** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "  #  " (Not solid)
- Step 2 (index 2): " ##  " (Not solid)
- Step 3 (index 4): " ### " (Not solid)
- Step 4 (index 1): "#### " (solid: first 4 are placed)
- Step 5 (index 5): "#####" (solid: first 5 are placed)
Total solid states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "   #" (Not solid)
- Step 2 (index 1): "#  #" (Not solid)
- Step 3 (index 2): "## #" (Not solid)
- Step 4 (index 3): "####" (solid)
Total solid states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was solid.

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
