## Title
Inventory Packing

## Slug
inventory-packing

## Difficulty
Medium

## Description
A packer groups items into boxes. Each item has a weight.

The Packer is working with a sequence of $n$ items, where the $i$-th item has a value of $a_i$.

The Packer needs to create a **packing list**. A packing list involves dividing the sequence of $n$ items into one or more contiguous boxes such that every item belongs to exactly one box.

For a specific packing list, the **weight limit** is calculated as follows:
1. Calculate the sum of values for each box in the partition.
2. The weight limit is the bitwise XOR sum of these box sums.

Your task is to calculate the bitwise XOR sum of the weight limit values of **all possible packing lists** of the sequence.

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
- Return a single integer representing the total XOR sum of weight limits of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
