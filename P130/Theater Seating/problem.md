## Title
Theater Seating

## Slug
theater-seating

## Difficulty
Medium

## Description
Patrons take seats. The row is 'packed' from the aisle if seats 1 to k are all occupied.

There is a sequence of $n$ seats indexed from $1$ to $n$. Initially, all seats are **empty**.

You fill the seats one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you fill the seat at the position `sequence[i-1]`.

A state is called **packed** if, after performing $k$ steps, exactly the first $k$ seats (indices $1$ to $k$) are occupied and all other seats are empty.

Your task is to calculate how many times the system becomes **packed** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "LLPLL" (Not packed)
- Step 2 (index 2): "LPPLL" (Not packed)
- Step 3 (index 4): "LPPPL" (Not packed)
- Step 4 (index 1): "PPPPL" (packed: first 4 are occupied)
- Step 5 (index 5): "PPPPP" (packed: first 5 are occupied)
Total packed states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "LLLP" (Not packed)
- Step 2 (index 1): "PLLP" (Not packed)
- Step 3 (index 2): "PPLP" (Not packed)
- Step 4 (index 3): "PPPP" (packed)
Total packed states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was packed.

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
