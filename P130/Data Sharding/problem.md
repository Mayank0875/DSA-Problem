## Title
Data Sharding

## Slug
data-sharding

## Difficulty
Medium

## Description
Database shards recover from a crash. The database is 'readable' up to shard k if all shards 1 to k are online.

There is a sequence of $n$ shards indexed from $1$ to $n$. Initially, all shards are **down**.

You recover the shards one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you recover the shard at the position `sequence[i-1]`.

A state is called **readable** if, after performing $k$ steps, exactly the first $k$ shards (indices $1$ to $k$) are up and all other shards are down.

Your task is to calculate how many times the system becomes **readable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "xxokxx" (Not readable)
- Step 2 (index 2): "xokokxx" (Not readable)
- Step 3 (index 4): "xokokokx" (Not readable)
- Step 4 (index 1): "okokokokx" (readable: first 4 are up)
- Step 5 (index 5): "okokokokok" (readable: first 5 are up)
Total readable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "xxxok" (Not readable)
- Step 2 (index 1): "okxxok" (Not readable)
- Step 3 (index 2): "okokxok" (Not readable)
- Step 4 (index 3): "okokokok" (readable)
Total readable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was readable.

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
