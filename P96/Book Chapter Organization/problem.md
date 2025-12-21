## Title
Book Chapter Organization

## Slug
book-chapter-organization

## Difficulty
Medium

## Description
An author groups written scenes into chapters. Each scene has a word count.

The Writer is working with a sequence of $n$ scenes, where the $i$-th scene has a value of $a_i$.

The Writer needs to create a **book outline**. A book outline involves dividing the sequence of $n$ scenes into one or more contiguous chapters such that every scene belongs to exactly one chapter.

For a specific book outline, the **pacing value** is calculated as follows:
1. Calculate the sum of values for each chapter in the partition.
2. The pacing value is the bitwise XOR sum of these chapter sums.

Your task is to calculate the bitwise XOR sum of the pacing value values of **all possible book outlines** of the sequence.

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
- Return a single integer representing the total XOR sum of pacing values of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
