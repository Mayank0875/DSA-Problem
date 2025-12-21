## Title
Library Bookshelf

## Slug
library-bookshelf

## Difficulty
Medium

## Description
A librarian groups books onto shelves. Each book has a thickness.

The Librarian is working with a sequence of $n$ books, where the $i$-th book has a value of $a_i$.

The Librarian needs to create a **shelving arrangement**. A shelving arrangement involves dividing the sequence of $n$ books into one or more contiguous shelves such that every book belongs to exactly one shelf.

For a specific shelving arrangement, the **shelf load** is calculated as follows:
1. Calculate the sum of values for each shelf in the partition.
2. The shelf load is the bitwise XOR sum of these shelf sums.

Your task is to calculate the bitwise XOR sum of the shelf load values of **all possible shelving arrangements** of the sequence.

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
- Return a single integer representing the total XOR sum of shelf loads of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
