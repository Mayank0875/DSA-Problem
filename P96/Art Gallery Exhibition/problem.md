## Title
Art Gallery Exhibition

## Slug
art-gallery-exhibition

## Difficulty
Medium

## Description
A curator groups paintings into themed rooms. Each painting has a value.

The Curator is working with a sequence of $n$ paintings, where the $i$-th painting has a value of $a_i$.

The Curator needs to create a **exhibition flow**. A exhibition flow involves dividing the sequence of $n$ paintings into one or more contiguous rooms such that every painting belongs to exactly one room.

For a specific exhibition flow, the **theme value** is calculated as follows:
1. Calculate the sum of values for each room in the partition.
2. The theme value is the bitwise XOR sum of these room sums.

Your task is to calculate the bitwise XOR sum of the theme value values of **all possible exhibition flows** of the sequence.

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
- Return a single integer representing the total XOR sum of theme values of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
