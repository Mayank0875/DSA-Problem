## Title
Crypto Block Chain

## Slug
crypto-block-chain

## Difficulty
Medium

## Description
A blockchain analyst compares two forks of a chain (block hashes). They need to identify the longest continuous sequence of blocks that is shared before the fork occurred (or after a merge). Find the length of this shared chain segment.

## Examples

### 1

#### Input
5
1 2 3 2 1
5
3 2 1 4 7

#### Output
3

#### Explanation
The longest common continuous sequence is `[3, 2, 1]`, which has a length of 3.

### 2

#### Input
5
0 0 0 0 0
5
0 0 0 0 0

#### Output
5

#### Explanation
Both sequences are identical. The longest common continuous segment is the entire sequence, length 5.

## Input Format
- The first line contains an integer `n`, the size of the first sequence.
- The second line contains `n` integers representing the first sequence.
- The third line contains an integer `m`, the size of the second sequence.
- The fourth line contains `m` integers representing the second sequence.

## Output Format
- Return a single integer representing the maximum length of a continuous segment that appears in both sequences.

## Constraints
- 1 ≤ n, m ≤ 1000
- 1 ≤ values ≤ 100

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, sliding-window
