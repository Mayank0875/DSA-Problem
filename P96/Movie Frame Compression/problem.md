## Title
Movie Frame Compression

## Slug
movie-frame-compression

## Difficulty
Medium

## Description
A codec groups frames into GOPs (Group of Pictures). Each frame has a data size.

The Codec is working with a sequence of $n$ frames, where the $i$-th frame has a value of $a_i$.

The Codec needs to create a **encoding stream**. A encoding stream involves dividing the sequence of $n$ frames into one or more contiguous GOPs such that every frame belongs to exactly one GOP.

For a specific encoding stream, the **bitrate target** is calculated as follows:
1. Calculate the sum of values for each GOP in the partition.
2. The bitrate target is the bitwise XOR sum of these GOP sums.

Your task is to calculate the bitwise XOR sum of the bitrate target values of **all possible encoding streams** of the sequence.

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
- Return a single integer representing the total XOR sum of bitrate targets of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
