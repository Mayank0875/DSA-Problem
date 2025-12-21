## Title
Digital Image Encoding

## Slug
digital-image-encoding

## Difficulty
Medium

## Description
An image encoder processes a row of pixels. Pixels are grouped into compression blocks.

The Encoder is working with a sequence of $n$ pixels, where the $i$-th pixel has a value of $a_i$.

The Encoder needs to create a **compression map**. A compression map involves dividing the sequence of $n$ pixels into one or more contiguous blocks such that every pixel belongs to exactly one block.

For a specific compression map, the **entropy value** is calculated as follows:
1. Calculate the sum of values for each block in the partition.
2. The entropy value is the bitwise XOR sum of these block sums.

Your task is to calculate the bitwise XOR sum of the entropy value values of **all possible compression maps** of the sequence.

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
- Return a single integer representing the total XOR sum of entropy values of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
