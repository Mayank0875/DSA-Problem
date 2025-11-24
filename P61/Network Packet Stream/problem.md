## Title
Network Packet Stream

## Slug
network-packet-stream

## Difficulty
Medium

## Description
A network sniffer captures a stream of data packets represented by characters. To detect a specific protocol header, the system looks for the longest sequence of unique packet identifiers (characters) arriving consecutively. Determine the length of this unique sequence.

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
