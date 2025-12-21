## Title
Financial Portfolio Strategy

## Slug
financial-portfolio-strategy

## Difficulty
Medium

## Description
An investor groups assets into diverse funds to manage risk. Each asset has a specific valuation.

The Analyst is working with a sequence of $n$ assets, where the $i$-th asset has a value of $a_i$.

The Analyst needs to create a **fund allocation**. A fund allocation involves dividing the sequence of $n$ assets into one or more contiguous funds such that every asset belongs to exactly one fund.

For a specific fund allocation, the **risk index** is calculated as follows:
1. Calculate the sum of values for each fund in the partition.
2. The risk index is the bitwise XOR sum of these fund sums.

Your task is to calculate the bitwise XOR sum of the risk index values of **all possible fund allocations** of the sequence.

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
- Return a single integer representing the total XOR sum of risk indexs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
