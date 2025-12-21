## Title
Historical Era Division

## Slug
historical-era-division

## Difficulty
Medium

## Description
A historian groups yearly events into eras. Each event has a significance score.

Professor Time is working with a sequence of $n$ events, where the $i$-th event has a value of $a_i$.

Professor Time needs to create a **timeline division**. A timeline division involves dividing the sequence of $n$ events into one or more contiguous eras such that every event belongs to exactly one era.

For a specific timeline division, the **historical impact** is calculated as follows:
1. Calculate the sum of values for each era in the partition.
2. The historical impact is the bitwise XOR sum of these era sums.

Your task is to calculate the bitwise XOR sum of the historical impact values of **all possible timeline divisions** of the sequence.

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
- Return a single integer representing the total XOR sum of historical impacts of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
