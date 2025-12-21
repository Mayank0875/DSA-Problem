## Title
Election Vote Count

## Slug
election-vote-count

## Difficulty
Medium

## Description
An official groups ballots into precincts. Each ballot has a candidate ID.

The Official is working with a sequence of $n$ ballots, where the $i$-th ballot has a value of $a_i$.

The Official needs to create a **district tally**. A district tally involves dividing the sequence of $n$ ballots into one or more contiguous precincts such that every ballot belongs to exactly one precinct.

For a specific district tally, the **vote margin** is calculated as follows:
1. Calculate the sum of values for each precinct in the partition.
2. The vote margin is the bitwise XOR sum of these precinct sums.

Your task is to calculate the bitwise XOR sum of the vote margin values of **all possible district tallys** of the sequence.

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
- Return a single integer representing the total XOR sum of vote margins of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
