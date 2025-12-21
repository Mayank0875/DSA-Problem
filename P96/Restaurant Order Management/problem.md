## Title
Restaurant Order Management

## Slug
restaurant-order-management

## Difficulty
Medium

## Description
A chef groups incoming orders into prep tickets. Each order has a preparation time.

Chef Ramsay is working with a sequence of $n$ orders, where the $i$-th order has a value of $a_i$.

Chef Ramsay needs to create a **ticket system**. A ticket system involves dividing the sequence of $n$ orders into one or more contiguous tickets such that every order belongs to exactly one ticket.

For a specific ticket system, the **service code** is calculated as follows:
1. Calculate the sum of values for each ticket in the partition.
2. The service code is the bitwise XOR sum of these ticket sums.

Your task is to calculate the bitwise XOR sum of the service code values of **all possible ticket systems** of the sequence.

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
- Return a single integer representing the total XOR sum of service codes of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
