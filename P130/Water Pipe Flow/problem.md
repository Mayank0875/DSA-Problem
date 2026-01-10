## Title
Water Pipe Flow

## Slug
water-pipe-flow

## Difficulty
Medium

## Description
Segments of a pipeline are welded. Water can 'flow' from the source (index 1) only if segments 1 to k are all welded.

There is a sequence of $n$ segments indexed from $1$ to $n$. Initially, all segments are **open**.

You weld the segments one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you weld the segment at the position `sequence[i-1]`.

A state is called **flowing** if, after performing $k$ steps, exactly the first $k$ segments (indices $1$ to $k$) are welded and all other segments are open.

Your task is to calculate how many times the system becomes **flowing** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "  -  " (Not flowing)
- Step 2 (index 2): " --  " (Not flowing)
- Step 3 (index 4): " --- " (Not flowing)
- Step 4 (index 1): "---- " (flowing: first 4 are welded)
- Step 5 (index 5): "-----" (flowing: first 5 are welded)
Total flowing states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "   -" (Not flowing)
- Step 2 (index 1): "-  -" (Not flowing)
- Step 3 (index 2): "-- -" (Not flowing)
- Step 4 (index 3): "----" (flowing)
Total flowing states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was flowing.

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
