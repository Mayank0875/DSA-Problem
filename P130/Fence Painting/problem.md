## Title
Fence Painting

## Slug
fence-painting

## Difficulty
Medium

## Description
Fence posts are painted. The fence looks 'finished' from the gate if posts 1 to k are all painted.

There is a sequence of $n$ posts indexed from $1$ to $n$. Initially, all posts are **bare**.

You paint the posts one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you paint the post at the position `sequence[i-1]`.

A state is called **finished** if, after performing $k$ steps, exactly the first $k$ posts (indices $1$ to $k$) are painted and all other posts are bare.

Your task is to calculate how many times the system becomes **finished** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "||I||" (Not finished)
- Step 2 (index 2): "|II||" (Not finished)
- Step 3 (index 4): "|III|" (Not finished)
- Step 4 (index 1): "IIII|" (finished: first 4 are painted)
- Step 5 (index 5): "IIIII" (finished: first 5 are painted)
Total finished states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "|||I" (Not finished)
- Step 2 (index 1): "I||I" (Not finished)
- Step 3 (index 2): "II|I" (Not finished)
- Step 4 (index 3): "IIII" (finished)
Total finished states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was finished.

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
