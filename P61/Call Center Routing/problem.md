## Title
Call Center Routing

## Slug
call-center-routing

## Difficulty
Medium

## Description
A system logs the department codes that handle a call. A complex issue is routed to many departments. Find the longest chain of transfers where the call was handled by a unique department at each step.

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
