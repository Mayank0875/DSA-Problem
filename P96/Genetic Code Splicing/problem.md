## Title
Genetic Code Splicing

## Slug
genetic-code-splicing

## Difficulty
Medium

## Description
A geneticist is analyzing a DNA strand. The strand is cut into gene segments for sequencing.

Dr. Helix is working with a sequence of $n$ nucleotides, where the $i$-th nucleotide has a value of $a_i$.

Dr. Helix needs to create a **sequencing layout**. A sequencing layout involves dividing the sequence of $n$ nucleotides into one or more contiguous segments such that every nucleotide belongs to exactly one segment.

For a specific sequencing layout, the **genetic marker** is calculated as follows:
1. Calculate the sum of values for each segment in the partition.
2. The genetic marker is the bitwise XOR sum of these segment sums.

Your task is to calculate the bitwise XOR sum of the genetic marker values of **all possible sequencing layouts** of the sequence.

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
- Return a single integer representing the total XOR sum of genetic markers of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
