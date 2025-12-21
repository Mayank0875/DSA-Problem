## Title
Music Album Tracklist

## Slug
music-album-tracklist

## Difficulty
Medium

## Description
A producer organizes recorded samples into tracks for an album. Each sample has a duration.

DJ Beat is working with a sequence of $n$ samples, where the $i$-th sample has a value of $a_i$.

DJ Beat needs to create a **album flow**. A album flow involves dividing the sequence of $n$ samples into one or more contiguous tracks such that every sample belongs to exactly one track.

For a specific album flow, the **vibe score** is calculated as follows:
1. Calculate the sum of values for each track in the partition.
2. The vibe score is the bitwise XOR sum of these track sums.

Your task is to calculate the bitwise XOR sum of the vibe score values of **all possible album flows** of the sequence.

## Examples

### 1

#### Input
1
1

#### Output
1

#### Explanation
Total XOR sum: 1.

### 2

#### Input
2
1 2

#### Output
0

#### Explanation
Partition {1}, {2}: Group sums are 1, 2. XOR sum = 1 ^ 2 = 3.
Partition {1, 2}: Group sum is 3. XOR sum = 3.
Total Result = 3 ^ 3 = 0.

## Input Format
- The first line contains a single integer $n$ — the length of the sequence.
- The second line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$.

## Output Format
- Return a single integer representing the total XOR sum of vibe scores of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
