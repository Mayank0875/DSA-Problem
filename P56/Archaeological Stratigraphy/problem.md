## Title
Archaeological Stratigraphy

## Slug
archaeological-stratigraphy

## Difficulty
Medium

## Description
Archaeologists compare the soil layers of two dig sites, represented by soil type IDs. They want to find the longest continuous sequence of layers that matches, indicating a shared geological era. Find the number of matching layers.

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
