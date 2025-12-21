## Title
Archaeological Dig

## Slug
archaeological-dig

## Difficulty
Medium

## Description
An archaeologist groups artifacts into grid squares. Each artifact has a value.

Dr. Jones is working with a sequence of $n$ artifacts, where the $i$-th artifact has a value of $a_i$.

Dr. Jones needs to create a **site grid**. A site grid involves dividing the sequence of $n$ artifacts into one or more contiguous squares such that every artifact belongs to exactly one square.

For a specific site grid, the **find value** is calculated as follows:
1. Calculate the sum of values for each square in the partition.
2. The find value is the bitwise XOR sum of these square sums.

Your task is to calculate the bitwise XOR sum of the find value values of **all possible site grids** of the sequence.

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
- Return a single integer representing the total XOR sum of find values of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
