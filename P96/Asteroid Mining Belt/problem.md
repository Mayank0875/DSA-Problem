## Title
Asteroid Mining Belt

## Slug
asteroid-mining-belt

## Difficulty
Medium

## Description
A miner groups asteroids into claim sectors. Each asteroid has an ore value.

The Miner is working with a sequence of $n$ asteroids, where the $i$-th asteroid has a value of $a_i$.

The Miner needs to create a **claim map**. A claim map involves dividing the sequence of $n$ asteroids into one or more contiguous sectors such that every asteroid belongs to exactly one sector.

For a specific claim map, the **yield estimate** is calculated as follows:
1. Calculate the sum of values for each sector in the partition.
2. The yield estimate is the bitwise XOR sum of these sector sums.

Your task is to calculate the bitwise XOR sum of the yield estimate values of **all possible claim maps** of the sequence.

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
- Return a single integer representing the total XOR sum of yield estimates of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
