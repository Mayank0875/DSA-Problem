## Title
Matching Socks Pair

## Slug
matching-socks-pair

## Difficulty
Easy

## Description
A laundry service is sorting a huge pile of socks. Each sock has a color code ID. The goal is to find pairs to pack. However, they are only interested in color codes where there are exactly two socks (a perfect pair) in the pile. If there is only one (missing match) or more than two (duplicates/extras), they are ignored. Return the color codes of the perfect pairs.

## Examples

### 1

#### Input
8
1 2 2 3 3 3 4 4

#### Output
2 4

#### Explanation
Value 2 appears twice. Value 4 appears twice. Value 3 appears three times (ignored). Value 1 appears once (ignored). The result is 2 and 4, sorted.

### 2

#### Input
5
5 5 5 6 7

#### Output


#### Explanation
Value 5 appears three times. Values 6 and 7 appear once. No value appears exactly twice.

## Input Format
- First line: integer n — number of elements.
- Second line: n space-separated integers.

## Output Format
- Return all integers that appear exactly twice in increasing order, as a list/array. If none, return an empty list/array.

## Constraints
- 1 ≤ n ≤ 10^5
- Values fit in 32-bit signed integer

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
hash-table, sorting
