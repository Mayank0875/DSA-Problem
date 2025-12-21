## Title
City Zoning Plan

## Slug
city-zoning-plan

## Difficulty
Medium

## Description
A planner groups city blocks into districts. Each block has a population count.

The Planner is working with a sequence of $n$ blocks, where the $i$-th block has a value of $a_i$.

The Planner needs to create a **zoning map**. A zoning map involves dividing the sequence of $n$ blocks into one or more contiguous districts such that every block belongs to exactly one district.

For a specific zoning map, the **population hash** is calculated as follows:
1. Calculate the sum of values for each district in the partition.
2. The population hash is the bitwise XOR sum of these district sums.

Your task is to calculate the bitwise XOR sum of the population hash values of **all possible zoning maps** of the sequence.

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
- Return a single integer representing the total XOR sum of population hashs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
