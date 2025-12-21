## Title
Battery Cell Array

## Slug
battery-cell-array

## Difficulty
Medium

## Description
An engineer groups battery cells into modules. Each cell has a voltage capacity.

The Engineer is working with a sequence of $n$ cells, where the $i$-th cell has a value of $a_i$.

The Engineer needs to create a **pack configuration**. A pack configuration involves dividing the sequence of $n$ cells into one or more contiguous modules such that every cell belongs to exactly one module.

For a specific pack configuration, the **power output** is calculated as follows:
1. Calculate the sum of values for each module in the partition.
2. The power output is the bitwise XOR sum of these module sums.

Your task is to calculate the bitwise XOR sum of the power output values of **all possible pack configurations** of the sequence.

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
- Return a single integer representing the total XOR sum of power outputs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
