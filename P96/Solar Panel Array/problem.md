## Title
Solar Panel Array

## Slug
solar-panel-array

## Difficulty
Medium

## Description
A technician groups panels into strings. Each panel has a wattage output.

The Technician is working with a sequence of $n$ panels, where the $i$-th panel has a value of $a_i$.

The Technician needs to create a **array wiring**. A array wiring involves dividing the sequence of $n$ panels into one or more contiguous strings such that every panel belongs to exactly one string.

For a specific array wiring, the **voltage sum** is calculated as follows:
1. Calculate the sum of values for each string in the partition.
2. The voltage sum is the bitwise XOR sum of these string sums.

Your task is to calculate the bitwise XOR sum of the voltage sum values of **all possible array wirings** of the sequence.

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
- Return a single integer representing the total XOR sum of voltage sums of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
