## Title
Browser History Session

## Slug
browser-history-session

## Difficulty
Medium

## Description
An analytics tool tracks the page types a user visits (e.g., 'H'ome, 'P'rofile, 'S'ettings). To measure exploration behavior, the tool calculates the length of the longest sequence of page visits where the user did not return to a previously visited page type within that sequence.

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
