## Title
Textile Weaving

## Slug
textile-weaving

## Difficulty
Medium

## Description
A weaver groups threads into bands. Each thread has a thickness.

The Weaver is working with a sequence of $n$ threads, where the $i$-th thread has a value of $a_i$.

The Weaver needs to create a **fabric pattern**. A fabric pattern involves dividing the sequence of $n$ threads into one or more contiguous bands such that every thread belongs to exactly one band.

For a specific fabric pattern, the **texture code** is calculated as follows:
1. Calculate the sum of values for each band in the partition.
2. The texture code is the bitwise XOR sum of these band sums.

Your task is to calculate the bitwise XOR sum of the texture code values of **all possible fabric patterns** of the sequence.

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
- Return a single integer representing the total XOR sum of texture codes of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
