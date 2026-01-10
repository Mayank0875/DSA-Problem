## Title
Pixel Display

## Slug
pixel-display

## Difficulty
Medium

## Description
Pixels on a line turn on. The line is 'solid' from the left if pixels 1 to k are all lit.

There is a sequence of $n$ pixels indexed from $1$ to $n$. Initially, all pixels are **black**.

You light up the pixels one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you light up the pixel at the position `sequence[i-1]`.

A state is called **solid** if, after performing $k$ steps, exactly the first $k$ pixels (indices $1$ to $k$) are lit and all other pixels are black.

Your task is to calculate how many times the system becomes **solid** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not solid)
- Step 2 (index 2): "01100" (Not solid)
- Step 3 (index 4): "01110" (Not solid)
- Step 4 (index 1): "11110" (solid: first 4 are lit)
- Step 5 (index 5): "11111" (solid: first 5 are lit)
Total solid states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not solid)
- Step 2 (index 1): "1001" (Not solid)
- Step 3 (index 2): "1101" (Not solid)
- Step 4 (index 3): "1111" (solid)
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
