## Title
Crypto Block Validation

## Slug
crypto-block-validation

## Difficulty
Medium

## Description
A miner groups transactions into blocks. Each transaction has a fee.

The Miner is working with a sequence of $n$ transactions, where the $i$-th transaction has a value of $a_i$.

The Miner needs to create a **blockchain segment**. A blockchain segment involves dividing the sequence of $n$ transactions into one or more contiguous blocks such that every transaction belongs to exactly one block.

For a specific blockchain segment, the **block hash** is calculated as follows:
1. Calculate the sum of values for each block in the partition.
2. The block hash is the bitwise XOR sum of these block sums.

Your task is to calculate the bitwise XOR sum of the block hash values of **all possible blockchain segments** of the sequence.

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
- Return a single integer representing the total XOR sum of block hashs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
