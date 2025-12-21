## Title
Call Center Queues

## Slug
call-center-queues

## Difficulty
Medium

## Description
A supervisor groups calls into shifts. Each call has a duration.

The Supervisor is working with a sequence of $n$ calls, where the $i$-th call has a value of $a_i$.

The Supervisor needs to create a **shift schedule**. A shift schedule involves dividing the sequence of $n$ calls into one or more contiguous shifts such that every call belongs to exactly one shift.

For a specific shift schedule, the **workload index** is calculated as follows:
1. Calculate the sum of values for each shift in the partition.
2. The workload index is the bitwise XOR sum of these shift sums.

Your task is to calculate the bitwise XOR sum of the workload index values of **all possible shift schedules** of the sequence.

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
- Return a single integer representing the total XOR sum of workload indexs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
