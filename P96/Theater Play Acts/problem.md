## Title
Theater Play Acts

## Slug
theater-play-acts

## Difficulty
Medium

## Description
A director groups scenes into acts. Each scene has a dramatic intensity.

The Director is working with a sequence of $n$ scenes, where the $i$-th scene has a value of $a_i$.

The Director needs to create a **play structure**. A play structure involves dividing the sequence of $n$ scenes into one or more contiguous acts such that every scene belongs to exactly one act.

For a specific play structure, the **drama score** is calculated as follows:
1. Calculate the sum of values for each act in the partition.
2. The drama score is the bitwise XOR sum of these act sums.

Your task is to calculate the bitwise XOR sum of the drama score values of **all possible play structures** of the sequence.

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
- Return a single integer representing the total XOR sum of drama scores of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
