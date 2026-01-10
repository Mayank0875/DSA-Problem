## Title
Railway Track Laying

## Slug
railway-track-laying

## Difficulty
Medium

## Description
Workers lay tracks on a route. The route is 'connected' from the depot (index 1) if all tracks from 1 to k are laid.

There is a sequence of $n$ tracks indexed from $1$ to $n$. Initially, all tracks are **empty**.

You lay the tracks one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you lay the track at the position `sequence[i-1]`.

A state is called **connected** if, after performing $k$ steps, exactly the first $k$ tracks (indices $1$ to $k$) are laid and all other tracks are empty.

Your task is to calculate how many times the system becomes **connected** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not connected)
- Step 2 (index 2): "01100" (Not connected)
- Step 3 (index 4): "01110" (Not connected)
- Step 4 (index 1): "11110" (connected: first 4 are laid)
- Step 5 (index 5): "11111" (connected: first 5 are laid)
Total connected states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not connected)
- Step 2 (index 1): "1001" (Not connected)
- Step 3 (index 2): "1101" (Not connected)
- Step 4 (index 3): "1111" (connected)
Total connected states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was connected.

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
