## Title
Submarine Sonar Pings

## Slug
submarine-sonar-pings

## Difficulty
Medium

## Description
A submarine detects sonar pings from different sources (chars). To identify a fleet, the operator looks for the longest sequence of pings where each one comes from a unique source.

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
