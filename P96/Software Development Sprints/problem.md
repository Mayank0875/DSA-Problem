## Title
Software Development Sprints

## Slug
software-development-sprints

## Difficulty
Medium

## Description
A manager groups tasks into sprints. Each task has story points.

The Scrum Master is working with a sequence of $n$ tasks, where the $i$-th task has a value of $a_i$.

The Scrum Master needs to create a **project roadmap**. A project roadmap involves dividing the sequence of $n$ tasks into one or more contiguous sprints such that every task belongs to exactly one sprint.

For a specific project roadmap, the **velocity target** is calculated as follows:
1. Calculate the sum of values for each sprint in the partition.
2. The velocity target is the bitwise XOR sum of these sprint sums.

Your task is to calculate the bitwise XOR sum of the velocity target values of **all possible project roadmaps** of the sequence.

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
- Return a single integer representing the total XOR sum of velocity targets of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
