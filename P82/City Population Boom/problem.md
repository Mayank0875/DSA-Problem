## Title
City Population Boom

## Slug
city-population-boom

## Difficulty
Easy

## Description
A demographer looks at n census records. They want to find periods of strictly increasing population.

You have population counts for n years.
A population boom consists of years where the population is strictly higher than the previously selected year.

You must analyze growth to find the longest possible population boom. You can skip any number of years to form the sequence, but you must maintain the original chronological order of the selected years. Calculate the maximum number of years that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest population booms (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 year.

## Input Format
- The first line contains an integer n: the number of years.
- The second line contains n integers x_1, x_2 ... x_n: the population of each year in order.

## Output Format
- Return one integer: the length of the longest valid population boom.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
