## Title
Social Media Feed

## Slug
social-media-feed

## Difficulty
Medium

## Description
An algorithm groups posts into sessions. Each post has an engagement score.

The Algorithm is working with a sequence of $n$ posts, where the $i$-th post has a value of $a_i$.

The Algorithm needs to create a **session view**. A session view involves dividing the sequence of $n$ posts into one or more contiguous sessions such that every post belongs to exactly one session.

For a specific session view, the **engagement metric** is calculated as follows:
1. Calculate the sum of values for each session in the partition.
2. The engagement metric is the bitwise XOR sum of these session sums.

Your task is to calculate the bitwise XOR sum of the engagement metric values of **all possible session views** of the sequence.

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
- Return a single integer representing the total XOR sum of engagement metrics of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
