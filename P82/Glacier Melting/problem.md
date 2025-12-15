## Title
Glacier Melting

## Slug
glacier-melting

## Difficulty
Easy

## Description
A scientist measures meltwater flow at n stations. They look for a cascade effect of strictly increasing flow.

You have flow rates for n stations.
A cascade consists of stations where flow rate is strictly higher than the previous station.

You must analyze the melt to find the longest possible melt cascade. You can skip any number of stations to form the sequence, but you must maintain the original downstream order of the selected stations. Calculate the maximum number of stations that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest melt cascades (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 station.

## Input Format
- The first line contains an integer n: the number of stations.
- The second line contains n integers x_1, x_2 ... x_n: the flow rate of each station in order.

## Output Format
- Return one integer: the length of the longest valid melt cascade.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
