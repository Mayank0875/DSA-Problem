## Title
Forest Conservation

## Slug
forest-conservation

## Difficulty
Medium

## Description
A ranger groups trees into conservation plots. Each tree has an age.

The Ranger is working with a sequence of $n$ trees, where the $i$-th tree has a value of $a_i$.

The Ranger needs to create a **forest map**. A forest map involves dividing the sequence of $n$ trees into one or more contiguous plots such that every tree belongs to exactly one plot.

For a specific forest map, the **age index** is calculated as follows:
1. Calculate the sum of values for each plot in the partition.
2. The age index is the bitwise XOR sum of these plot sums.

Your task is to calculate the bitwise XOR sum of the age index values of **all possible forest maps** of the sequence.

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
- Return a single integer representing the total XOR sum of age indexs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
