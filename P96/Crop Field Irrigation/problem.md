## Title
Crop Field Irrigation

## Slug
crop-field-irrigation

## Difficulty
Medium

## Description
A farmer divides a row of crops into irrigation zones. Each crop needs a specific amount of water.

Farmer John is working with a sequence of $n$ crops, where the $i$-th crop has a value of $a_i$.

Farmer John needs to create a **irrigation plan**. A irrigation plan involves dividing the sequence of $n$ crops into one or more contiguous zones such that every crop belongs to exactly one zone.

For a specific irrigation plan, the **water usage code** is calculated as follows:
1. Calculate the sum of values for each zone in the partition.
2. The water usage code is the bitwise XOR sum of these zone sums.

Your task is to calculate the bitwise XOR sum of the water usage code values of **all possible irrigation plans** of the sequence.

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
- Return a single integer representing the total XOR sum of water usage codes of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
