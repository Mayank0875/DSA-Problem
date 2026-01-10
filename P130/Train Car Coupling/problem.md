## Title
Train Car Coupling

## Slug
train-car-coupling

## Difficulty
Medium

## Description
Cars connect to the engine. The train is 'ready' up to car k if all cars 1 to k are coupled.

There is a sequence of $n$ cars indexed from $1$ to $n$. Initially, all cars are **detached**.

You attach the cars one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you attach the car at the position `sequence[i-1]`.

A state is called **ready** if, after performing $k$ steps, exactly the first $k$ cars (indices $1$ to $k$) are coupled and all other cars are detached.

Your task is to calculate how many times the system becomes **ready** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "  []  " (Not ready)
- Step 2 (index 2): " [][]  " (Not ready)
- Step 3 (index 4): " [][][] " (Not ready)
- Step 4 (index 1): "[][][][] " (ready: first 4 are coupled)
- Step 5 (index 5): "[][][][][]" (ready: first 5 are coupled)
Total ready states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "   []" (Not ready)
- Step 2 (index 1): "[]  []" (Not ready)
- Step 3 (index 2): "[][] []" (Not ready)
- Step 4 (index 3): "[][][][]" (ready)
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
