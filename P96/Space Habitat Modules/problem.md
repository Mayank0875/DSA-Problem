## Title
Space Habitat Modules

## Slug
space-habitat-modules

## Difficulty
Medium

## Description
An architect groups habitat pods into wings. Each pod has an oxygen requirement.

The Architect is working with a sequence of $n$ pods, where the $i$-th pod has a value of $a_i$.

The Architect needs to create a **station blueprint**. A station blueprint involves dividing the sequence of $n$ pods into one or more contiguous wings such that every pod belongs to exactly one wing.

For a specific station blueprint, the **life support load** is calculated as follows:
1. Calculate the sum of values for each wing in the partition.
2. The life support load is the bitwise XOR sum of these wing sums.

Your task is to calculate the bitwise XOR sum of the life support load values of **all possible station blueprints** of the sequence.

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
- Return a single integer representing the total XOR sum of life support loads of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
