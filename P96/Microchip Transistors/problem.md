## Title
Microchip Transistors

## Slug
microchip-transistors

## Difficulty
Medium

## Description
A designer groups transistors into logic gates. Each transistor has a switching speed.

The Designer is working with a sequence of $n$ transistors, where the $i$-th transistor has a value of $a_i$.

The Designer needs to create a **circuit block**. A circuit block involves dividing the sequence of $n$ transistors into one or more contiguous gates such that every transistor belongs to exactly one gate.

For a specific circuit block, the **clock cycle** is calculated as follows:
1. Calculate the sum of values for each gate in the partition.
2. The clock cycle is the bitwise XOR sum of these gate sums.

Your task is to calculate the bitwise XOR sum of the clock cycle values of **all possible circuit blocks** of the sequence.

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
- Return a single integer representing the total XOR sum of clock cycles of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
