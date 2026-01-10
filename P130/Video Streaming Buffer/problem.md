## Title
Video Streaming Buffer

## Slug
video-streaming-buffer

## Difficulty
Medium

## Description
Video segments buffer randomly. The video plays 'smoothly' if segments 1 to k are all buffered.

There is a sequence of $n$ segments indexed from $1$ to $n$. Initially, all segments are **buffering**.

You buffer the segments one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you buffer the segment at the position `sequence[i-1]`.

A state is called **smooth** if, after performing $k$ steps, exactly the first $k$ segments (indices $1$ to $k$) are ready and all other segments are buffering.

Your task is to calculate how many times the system becomes **smooth** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "..|.." (Not smooth)
- Step 2 (index 2): ".||.." (Not smooth)
- Step 3 (index 4): ".|||." (Not smooth)
- Step 4 (index 1): "||||." (smooth: first 4 are ready)
- Step 5 (index 5): "|||||" (smooth: first 5 are ready)
Total smooth states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "...|" (Not smooth)
- Step 2 (index 1): "|..|" (Not smooth)
- Step 3 (index 2): "||.|" (Not smooth)
- Step 4 (index 3): "||||" (smooth)
Total smooth states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was smooth.

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
