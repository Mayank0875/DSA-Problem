## Title
Signal Processing

## Slug
signal-processing

## Difficulty
Medium

## Description
An engineer groups signal pulses into messages. Each pulse has an amplitude.

The Engineer is working with a sequence of $n$ pulses, where the $i$-th pulse has a value of $a_i$.

The Engineer needs to create a **transmission stream**. A transmission stream involves dividing the sequence of $n$ pulses into one or more contiguous messages such that every pulse belongs to exactly one message.

For a specific transmission stream, the **signal strength** is calculated as follows:
1. Calculate the sum of values for each message in the partition.
2. The signal strength is the bitwise XOR sum of these message sums.

Your task is to calculate the bitwise XOR sum of the signal strength values of **all possible transmission streams** of the sequence.

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
- Return a single integer representing the total XOR sum of signal strengths of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
