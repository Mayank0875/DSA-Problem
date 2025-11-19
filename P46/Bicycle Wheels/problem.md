## Title
Bicycle Wheels

## Slug
bicycle-wheels

## Difficulty
Easy

## Description
A bicycle factory tracks component IDs. Each standard bicycle requires exactly two wheels of the same model ID. The inventory system checks the assembly line log. Identify which wheel model IDs were used exactly twice (indicating one complete bike was assembled with them).

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
