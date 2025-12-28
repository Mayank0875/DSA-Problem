## Title
Genetic Fragment Splicing

## Slug
genetic-fragment-splicing

## Difficulty
Medium

## Description
A geneticist aligns DNA fragments. Each fragment covers a specific range of base pair indices.

The sample has list of fragments, each defined by a start index and an end index, represented as a pair `[start, end]`.

To form a valid non-overlapping sequence, the end index of a fragment must be strictly less than the start index of the next. Specifically, to transition from fragment `[a, b]` to a subsequent fragment `[c, d]`, the end of the first fragment must be **strictly less than** the start of the second fragment (i.e., `b < c`).

You can select fragments in any order you like to form a valid gene sequence. Your goal is to determine the maximum number of fragments that can be included in a single gene sequence.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest gene sequence is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The fragments can be reordered to form the gene sequence `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available fragments.
- The next `n` lines each contain two integers, representing the `start` and `end` of an fragment.

## Output Format
- Return a single integer representing the maximum length of the gene sequence.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
