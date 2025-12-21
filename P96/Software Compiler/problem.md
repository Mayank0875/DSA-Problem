## Title
Software Compiler

## Slug
software-compiler

## Difficulty
Medium

## Description
A compiler groups code tokens into statements. Each token has a type ID.

The Compiler is working with a sequence of $n$ tokens, where the $i$-th token has a value of $a_i$.

The Compiler needs to create a **parse tree**. A parse tree involves dividing the sequence of $n$ tokens into one or more contiguous statements such that every token belongs to exactly one statement.

For a specific parse tree, the **syntax hash** is calculated as follows:
1. Calculate the sum of values for each statement in the partition.
2. The syntax hash is the bitwise XOR sum of these statement sums.

Your task is to calculate the bitwise XOR sum of the syntax hash values of **all possible parse trees** of the sequence.

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
- Return a single integer representing the total XOR sum of syntax hashs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
