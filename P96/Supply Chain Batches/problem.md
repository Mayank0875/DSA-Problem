## Title
Supply Chain Batches

## Slug
supply-chain-batches

## Difficulty
Medium

## Description
A factory produces items on a conveyor belt. Items are grouped into batches for shipping.

The Foreman is working with a sequence of $n$ items, where the $i$-th item has a value of $a_i$.

The Foreman needs to create a **shipping schedule**. A shipping schedule involves dividing the sequence of $n$ items into one or more contiguous batches such that every item belongs to exactly one batch.

For a specific shipping schedule, the **batch ID** is calculated as follows:
1. Calculate the sum of values for each batch in the partition.
2. The batch ID is the bitwise XOR sum of these batch sums.

Your task is to calculate the bitwise XOR sum of the batch ID values of **all possible shipping schedules** of the sequence.

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
- Return a single integer representing the total XOR sum of batch IDs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
