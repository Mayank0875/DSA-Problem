## Title
Network Packet Header

## Slug
network-packet-header

## Difficulty
Hard

## Description
Network packets have headers. A header is considered malformed if the checksum contains adjacent duplicate digits.

For example, the header checksum `12321` is valid because no two adjacent digits are the same. However, `1223` is invalid because the digit `2` appears twice consecutively.

You are given a range of header checksums from $a$ to $b$ (inclusive). Your task is to calculate exactly how many header checksums in this range satisfy this condition.

## Examples

### 1

#### Input
123 321

#### Output
171

#### Explanation
There are 171 valid header checksums between 123 and 321 (inclusive).

### 2

#### Input
1234 1234

#### Output
1

#### Explanation
The number 1234 is valid.

## Input Format
- The input contains two space-separated integers, $a$ and $b$.

## Output Format
- Return a single integer representing the count of valid header checksums in the range $[a, b]$.

## Constraints
- 0 ≤ a ≤ b ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
