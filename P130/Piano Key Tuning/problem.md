## Title
Piano Key Tuning

## Slug
piano-key-tuning

## Difficulty
Medium

## Description
A tuner tunes keys 1 to n. The piano is 'playable' in the lower register if keys 1 to k are all tuned.

There is a sequence of $n$ keys indexed from $1$ to $n$. Initially, all keys are **untuned**.

You tune the keys one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you tune the key at the position `sequence[i-1]`.

A state is called **playable** if, after performing $k$ steps, exactly the first $k$ keys (indices $1$ to $k$) are tuned and all other keys are untuned.

Your task is to calculate how many times the system becomes **playable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "xx!xx" (Not playable)
- Step 2 (index 2): "x!!xx" (Not playable)
- Step 3 (index 4): "x!!!x" (Not playable)
- Step 4 (index 1): "!!!!x" (playable: first 4 are tuned)
- Step 5 (index 5): "!!!!!" (playable: first 5 are tuned)
Total playable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "xxx!" (Not playable)
- Step 2 (index 1): "!xx!" (Not playable)
- Step 3 (index 2): "!!x!" (Not playable)
- Step 4 (index 3): "!!!!" (playable)
Total playable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was playable.

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
