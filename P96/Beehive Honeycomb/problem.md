## Title
Beehive Honeycomb

## Slug
beehive-honeycomb

## Difficulty
Medium

## Description
A bee groups nectar drops into cells. Each drop has a sugar content.

The Worker Bee is working with a sequence of $n$ drops, where the $i$-th drop has a value of $a_i$.

The Worker Bee needs to create a **comb section**. A comb section involves dividing the sequence of $n$ drops into one or more contiguous cells such that every drop belongs to exactly one cell.

For a specific comb section, the **honey quality** is calculated as follows:
1. Calculate the sum of values for each cell in the partition.
2. The honey quality is the bitwise XOR sum of these cell sums.

Your task is to calculate the bitwise XOR sum of the honey quality values of **all possible comb sections** of the sequence.

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
- Return a single integer representing the total XOR sum of honey qualitys of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
