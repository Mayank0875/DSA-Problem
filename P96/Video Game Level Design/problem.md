## Title
Video Game Level Design

## Slug
video-game-level-design

## Difficulty
Medium

## Description
A designer groups obstacles into level sectors. Each obstacle has a difficulty rating.

The Designer is working with a sequence of $n$ obstacles, where the $i$-th obstacle has a value of $a_i$.

The Designer needs to create a **level layout**. A level layout involves dividing the sequence of $n$ obstacles into one or more contiguous sectors such that every obstacle belongs to exactly one sector.

For a specific level layout, the **difficulty hash** is calculated as follows:
1. Calculate the sum of values for each sector in the partition.
2. The difficulty hash is the bitwise XOR sum of these sector sums.

Your task is to calculate the bitwise XOR sum of the difficulty hash values of **all possible level layouts** of the sequence.

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
- Return a single integer representing the total XOR sum of difficulty hashs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
