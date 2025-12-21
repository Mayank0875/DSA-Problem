## Title
Chemical Reaction Chains

## Slug
chemical-reaction-chains

## Difficulty
Medium

## Description
A chemist groups reaction steps into stages. Each step releases energy.

The Chemist is working with a sequence of $n$ steps, where the $i$-th step has a value of $a_i$.

The Chemist needs to create a **reaction process**. A reaction process involves dividing the sequence of $n$ steps into one or more contiguous stages such that every step belongs to exactly one stage.

For a specific reaction process, the **energy signature** is calculated as follows:
1. Calculate the sum of values for each stage in the partition.
2. The energy signature is the bitwise XOR sum of these stage sums.

Your task is to calculate the bitwise XOR sum of the energy signature values of **all possible reaction processs** of the sequence.

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
- Return a single integer representing the total XOR sum of energy signatures of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
