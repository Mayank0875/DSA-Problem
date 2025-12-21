## Title
Glacier Ice Core

## Slug
glacier-ice-core

## Difficulty
Medium

## Description
A scientist groups ice layers into years. Each layer has a CO2 concentration.

The Scientist is working with a sequence of $n$ layers, where the $i$-th layer has a value of $a_i$.

The Scientist needs to create a **climate record**. A climate record involves dividing the sequence of $n$ layers into one or more contiguous years such that every layer belongs to exactly one year.

For a specific climate record, the **carbon marker** is calculated as follows:
1. Calculate the sum of values for each year in the partition.
2. The carbon marker is the bitwise XOR sum of these year sums.

Your task is to calculate the bitwise XOR sum of the carbon marker values of **all possible climate records** of the sequence.

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
- Return a single integer representing the total XOR sum of carbon markers of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
