## Title
Star Rating Trends

## Slug
star-rating-trends

## Difficulty
Easy

## Description
A review platform analyzes user rating trends. A 'stable trend' is defined as a sequence of $n$ ratings (using 1 to 5 stars) where the ratings never decrease over time. For example, '1-1-3-5' is stable, but '3-2-5' is not. Given the length of the trend $n$, calculate how many distinct stable rating sequences can be formed.

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
