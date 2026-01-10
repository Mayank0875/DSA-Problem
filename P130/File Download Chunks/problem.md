## Title
File Download Chunks

## Slug
file-download-chunks

## Difficulty
Medium

## Description
A file is downloaded in numbered chunks. The file is 'playable' up to a certain point only if all chunks from the start up to that point have arrived.

There is a sequence of $n$ chunks indexed from $1$ to $n$. Initially, all chunks are **pending**.

You download the chunks one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you download the chunk at the position `sequence[i-1]`.

A state is called **playable** if, after performing $k$ steps, exactly the first $k$ chunks (indices $1$ to $k$) are downloaded and all other chunks are pending.

Your task is to calculate how many times the system becomes **playable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not playable)
- Step 2 (index 2): "01100" (Not playable)
- Step 3 (index 4): "01110" (Not playable)
- Step 4 (index 1): "11110" (playable: first 4 are downloaded)
- Step 5 (index 5): "11111" (playable: first 5 are downloaded)
Total playable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not playable)
- Step 2 (index 1): "1001" (Not playable)
- Step 3 (index 2): "1101" (Not playable)
- Step 4 (index 3): "1111" (playable)
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
