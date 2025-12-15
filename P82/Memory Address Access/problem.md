## Title
Memory Address Access

## Slug
memory-address-access

## Difficulty
Easy

## Description
A CPU accesses n memory addresses. Optimization is best for strictly increasing access patterns.

You have a log of n memory addresses.
A sequential access pattern consists of addresses where the value is strictly higher than the previous access.

You must optimize trace to find the longest possible access pattern. You can skip any number of addresses to form the sequence, but you must maintain the original execution order order of the selected addresses. Calculate the maximum number of addresses that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest access patterns (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 address.

## Input Format
- The first line contains an integer n: the number of addresses.
- The second line contains n integers x_1, x_2 ... x_n: the address value of each address in order.

## Output Format
- Return one integer: the length of the longest valid access pattern.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
