## Title
Classroom Seating

## Slug
classroom-seating

## Difficulty
Medium

## Description
A teacher groups desks into rows. Each student at a desk has a grade.

The Teacher is working with a sequence of $n$ students, where the $i$-th student has a value of $a_i$.

The Teacher needs to create a **seating chart**. A seating chart involves dividing the sequence of $n$ students into one or more contiguous rows such that every student belongs to exactly one row.

For a specific seating chart, the **class performance** is calculated as follows:
1. Calculate the sum of values for each row in the partition.
2. The class performance is the bitwise XOR sum of these row sums.

Your task is to calculate the bitwise XOR sum of the class performance values of **all possible seating charts** of the sequence.

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
- Return a single integer representing the total XOR sum of class performances of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
