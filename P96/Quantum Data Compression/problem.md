## Title
Quantum Data Compression

## Slug
quantum-data-compression

## Difficulty
Medium

## Description
A quantum computer processes a stream of qubits. Data must be segmented into packets for transmission.

The Quantum Engineer is working with a sequence of $n$ qubits, where the $i$-th qubit has a value of $a_i$.

The Quantum Engineer needs to create a **transmission scheme**. A transmission scheme involves dividing the sequence of $n$ qubits into one or more contiguous packets such that every qubit belongs to exactly one packet.

For a specific transmission scheme, the **transmission hash** is calculated as follows:
1. Calculate the sum of values for each packet in the partition.
2. The transmission hash is the bitwise XOR sum of these packet sums.

Your task is to calculate the bitwise XOR sum of the transmission hash values of **all possible transmission schemes** of the sequence.

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
- Return a single integer representing the total XOR sum of transmission hashs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
