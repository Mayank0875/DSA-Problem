## Title
Server Log Analysis

## Slug
server-log-analysis

## Difficulty
Medium

## Description
A sysadmin groups log entries into events. Each entry has a severity level.

The Sysadmin is working with a sequence of $n$ entries, where the $i$-th entry has a value of $a_i$.

The Sysadmin needs to create a **event log**. A event log involves dividing the sequence of $n$ entries into one or more contiguous events such that every entry belongs to exactly one event.

For a specific event log, the **alert level** is calculated as follows:
1. Calculate the sum of values for each event in the partition.
2. The alert level is the bitwise XOR sum of these event sums.

Your task is to calculate the bitwise XOR sum of the alert level values of **all possible event logs** of the sequence.

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
- Return a single integer representing the total XOR sum of alert levels of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
