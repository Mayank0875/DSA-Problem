## Title
Geological Strata

## Slug
geological-strata

## Difficulty
Medium

## Description
A geologist groups soil layers into epochs. Each layer has a density.

The Geologist is working with a sequence of $n$ layers, where the $i$-th layer has a value of $a_i$.

The Geologist needs to create a **stratigraphy chart**. A stratigraphy chart involves dividing the sequence of $n$ layers into one or more contiguous epochs such that every layer belongs to exactly one epoch.

For a specific stratigraphy chart, the **density profile** is calculated as follows:
1. Calculate the sum of values for each epoch in the partition.
2. The density profile is the bitwise XOR sum of these epoch sums.

Your task is to calculate the bitwise XOR sum of the density profile values of **all possible stratigraphy charts** of the sequence.

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
- Return a single integer representing the total XOR sum of density profiles of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
