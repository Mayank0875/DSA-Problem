## Title
Hotel Room Cleaning

## Slug
hotel-room-cleaning

## Difficulty
Medium

## Description
Rooms 1 to n are cleaned. The corridor is 'ready' if rooms 1 to k are all clean.

There is a sequence of $n$ rooms indexed from $1$ to $n$. Initially, all rooms are **dirty**.

You clean the rooms one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you clean the room at the position `sequence[i-1]`.

A state is called **ready** if, after performing $k$ steps, exactly the first $k$ rooms (indices $1$ to $k$) are clean and all other rooms are dirty.

Your task is to calculate how many times the system becomes **ready** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "xxcxx" (Not ready)
- Step 2 (index 2): "xccxx" (Not ready)
- Step 3 (index 4): "xcccx" (Not ready)
- Step 4 (index 1): "ccccx" (ready: first 4 are clean)
- Step 5 (index 5): "ccccc" (ready: first 5 are clean)
Total ready states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "xxxc" (Not ready)
- Step 2 (index 1): "cxxc" (Not ready)
- Step 3 (index 2): "ccxc" (Not ready)
- Step 4 (index 3): "cccc" (ready)
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
