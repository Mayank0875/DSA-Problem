## Title
Traveling Salesman Route

## Slug
traveling-salesman-route

## Difficulty
Medium

## Description
A traveler logs the city codes of every city they visit in order. They want to find the longest leg of their journey where they did not visit the same city twice. Given the log string, calculate the number of cities in this unique leg.

## Examples

### 1

#### Input
abcabcbb

#### Output
3

#### Explanation
The answer is "abc", with the length of 3.

### 2

#### Input
bbbbb

#### Output
1

#### Explanation
The answer is "b", with the length of 1.

## Input Format
- The input consists of a single line containing the string `s`.

## Output Format
- Return a single integer representing the maximum length of a substring with unique characters.

## Constraints
- 1 ≤ length(s) ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, hash-table, sliding-window
