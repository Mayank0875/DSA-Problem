## Title
Survey Response Patterns

## Slug
survey-response-patterns

## Difficulty
Easy

## Description
A survey asks $n$ questions. The answers are on a 5-point scale: 'Strongly Disagree', 'Disagree', 'Neutral', 'Agree', 'Strongly Agree'. An analyst looks for 'optimistic' respondents whose answers never become more negative as the survey progresses (non-decreasing scale). How many such response patterns exist?

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
