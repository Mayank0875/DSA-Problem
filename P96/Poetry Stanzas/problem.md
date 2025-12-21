## Title
Poetry Stanzas

## Slug
poetry-stanzas

## Difficulty
Medium

## Description
A poet arranges lines of verse into stanzas. Each line has a syllable count.

The Poet is working with a sequence of $n$ lines, where the $i$-th line has a value of $a_i$.

The Poet needs to create a **poem structure**. A poem structure involves dividing the sequence of $n$ lines into one or more contiguous stanzas such that every line belongs to exactly one stanza.

For a specific poem structure, the **rhythm key** is calculated as follows:
1. Calculate the sum of values for each stanza in the partition.
2. The rhythm key is the bitwise XOR sum of these stanza sums.

Your task is to calculate the bitwise XOR sum of the rhythm key values of **all possible poem structures** of the sequence.

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
- Return a single integer representing the total XOR sum of rhythm keys of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
