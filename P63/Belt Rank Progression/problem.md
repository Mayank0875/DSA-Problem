## Title
Belt Rank Progression

## Slug
belt-rank-progression

## Difficulty
Easy

## Description
A martial arts dojo has 5 belt ranks: White, Yellow, Green, Blue, Black. A student records their belt color at the end of each of their first $n$ years. Since belt rank cannot go down, the sequence must be non-decreasing. Calculate the number of possible belt histories for a student over $n$ years.

## Examples

### 1

#### Input
1

#### Output
5

#### Explanation
There are 5 valid sequences of length 1.

### 2

#### Input
2

#### Output
15

#### Explanation
There are 15 valid sorted sequences of length 2 (e.g., aa, ae, ai, ao, au, ee, etc.).

## Input Format
- The input consists of a single integer n, representing the required length/quantity.

## Output Format
- Return a single integer representing the total number of valid sorted sequences.

## Constraints
- 1 ≤ n ≤ 50

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math
