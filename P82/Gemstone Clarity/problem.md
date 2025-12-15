## Title
Gemstone Clarity

## Slug
gemstone-clarity

## Difficulty
Easy

## Description
A jeweler inspects n gems in a row. They want to create a necklace where clarity improves with each gem.

You have clarity scores for n gems.
A graded necklace consists of gems where the clarity is strictly higher than the previous gem.

You must select gems to find the longest possible graded necklace. You can skip any number of gems to form the sequence, but you must maintain the original arrangement order of the selected gems. Calculate the maximum number of gems that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest graded necklaces (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 gem.

## Input Format
- The first line contains an integer n: the number of gems.
- The second line contains n integers x_1, x_2 ... x_n: the clarity of each gem in order.

## Output Format
- Return one integer: the length of the longest valid graded necklace.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
