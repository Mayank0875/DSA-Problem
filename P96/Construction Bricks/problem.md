## Title
Construction Bricks

## Slug
construction-bricks

## Difficulty
Medium

## Description
A mason groups bricks into courses (rows). Each brick has a weight.

The Mason is working with a sequence of $n$ bricks, where the $i$-th brick has a value of $a_i$.

The Mason needs to create a **wall section**. A wall section involves dividing the sequence of $n$ bricks into one or more contiguous courses such that every brick belongs to exactly one course.

For a specific wall section, the **structural load** is calculated as follows:
1. Calculate the sum of values for each course in the partition.
2. The structural load is the bitwise XOR sum of these course sums.

Your task is to calculate the bitwise XOR sum of the structural load values of **all possible wall sections** of the sequence.

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
- Return a single integer representing the total XOR sum of structural loads of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
