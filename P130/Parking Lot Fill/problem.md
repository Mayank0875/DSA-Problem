## Title
Parking Lot Fill

## Slug
parking-lot-fill

## Difficulty
Medium

## Description
Cars park in spots 1 to n. The row is 'full' up to k if spots 1 to k are taken.

There is a sequence of $n$ spots indexed from $1$ to $n$. Initially, all spots are **free**.

You occupy the spots one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you occupy the spot at the position `sequence[i-1]`.

A state is called **full** if, after performing $k$ steps, exactly the first $k$ spots (indices $1$ to $k$) are taken and all other spots are free.

Your task is to calculate how many times the system becomes **full** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "  C  " (Not full)
- Step 2 (index 2): " CC  " (Not full)
- Step 3 (index 4): " CCC " (Not full)
- Step 4 (index 1): "CCCC " (full: first 4 are taken)
- Step 5 (index 5): "CCCCC" (full: first 5 are taken)
Total full states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "   C" (Not full)
- Step 2 (index 1): "C  C" (Not full)
- Step 3 (index 2): "CC C" (Not full)
- Step 4 (index 3): "CCCC" (full)
Total full states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was full.

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
