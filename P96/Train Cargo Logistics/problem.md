## Title
Train Cargo Logistics

## Slug
train-cargo-logistics

## Difficulty
Medium

## Description
A freight train is loaded with containers of varying weights. The train cars must be coupled in a specific way.

The Yardmaster is working with a sequence of $n$ containers, where the $i$-th container has a value of $a_i$.

The Yardmaster needs to create a **coupling plan**. A coupling plan involves dividing the sequence of $n$ containers into one or more contiguous cars such that every container belongs to exactly one car.

For a specific coupling plan, the **load signature** is calculated as follows:
1. Calculate the sum of values for each car in the partition.
2. The load signature is the bitwise XOR sum of these car sums.

Your task is to calculate the bitwise XOR sum of the load signature values of **all possible coupling plans** of the sequence.

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
- Return a single integer representing the total XOR sum of load signatures of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
