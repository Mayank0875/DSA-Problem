## Title
Recipe Ingredients

## Slug
recipe-ingredients

## Difficulty
Medium

## Description
A cook groups ingredients into prep bowls. Each ingredient has a calorie count.

The Cook is working with a sequence of $n$ ingredients, where the $i$-th ingredient has a value of $a_i$.

The Cook needs to create a **mise en place**. A mise en place involves dividing the sequence of $n$ ingredients into one or more contiguous bowls such that every ingredient belongs to exactly one bowl.

For a specific mise en place, the **nutrition profile** is calculated as follows:
1. Calculate the sum of values for each bowl in the partition.
2. The nutrition profile is the bitwise XOR sum of these bowl sums.

Your task is to calculate the bitwise XOR sum of the nutrition profile values of **all possible mise en places** of the sequence.

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
- Return a single integer representing the total XOR sum of nutrition profiles of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
