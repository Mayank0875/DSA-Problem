## Title
Robot Swarm Logic

## Slug
robot-swarm-logic

## Difficulty
Medium

## Description
A controller groups robots into squads. Each robot has a battery level.

The Controller is working with a sequence of $n$ robots, where the $i$-th robot has a value of $a_i$.

The Controller needs to create a **swarm formation**. A swarm formation involves dividing the sequence of $n$ robots into one or more contiguous squads such that every robot belongs to exactly one squad.

For a specific swarm formation, the **power reserve** is calculated as follows:
1. Calculate the sum of values for each squad in the partition.
2. The power reserve is the bitwise XOR sum of these squad sums.

Your task is to calculate the bitwise XOR sum of the power reserve values of **all possible swarm formations** of the sequence.

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
- Return a single integer representing the total XOR sum of power reserves of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
