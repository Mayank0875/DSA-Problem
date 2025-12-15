## Title
Tree Rings

## Slug
tree-rings

## Difficulty
Easy

## Description
A dendrologist measures n tree rings. They want to find a period of strictly increasing growth width.

You have widths of n tree rings.
A growth period consists of rings where the width is strictly wider than the previous ring.

You must study the sample to find the longest possible growth period. You can skip any number of rings to form the sequence, but you must maintain the original age order of the selected rings. Calculate the maximum number of rings that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest growth periods (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 ring.

## Input Format
- The first line contains an integer n: the number of rings.
- The second line contains n integers x_1, x_2 ... x_n: the width of each ring in order.

## Output Format
- Return one integer: the length of the longest valid growth period.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
