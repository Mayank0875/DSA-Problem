## Title
Traffic Light Cycles

## Slug
traffic-light-cycles

## Difficulty
Medium

## Description
A traffic engineer groups seconds of flow into green light phases. Each second has a vehicle count.

The Engineer is working with a sequence of $n$ seconds, where the $i$-th second has a value of $a_i$.

The Engineer needs to create a **signal program**. A signal program involves dividing the sequence of $n$ seconds into one or more contiguous phases such that every second belongs to exactly one phase.

For a specific signal program, the **flow efficiency** is calculated as follows:
1. Calculate the sum of values for each phase in the partition.
2. The flow efficiency is the bitwise XOR sum of these phase sums.

Your task is to calculate the bitwise XOR sum of the flow efficiency values of **all possible signal programs** of the sequence.

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
- Return a single integer representing the total XOR sum of flow efficiencys of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
