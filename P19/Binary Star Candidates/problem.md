## Title

Binary Star Candidates

## Slug

binary-star-candidates

## Difficulty

Easy

## Description

An astronomer is scanning a star cluster. Each star is given a 'type' ID. A 'binary candidate' is a star type that appears exactly twice in the scan, suggesting a pair. Given the list of star type IDs, find all binary candidates. Return them in increasing order. If no type appears exactly twice, return an empty list.

## Examples

### 1
#### Input
8
1 2 2 3 3 3 4 4

#### Output
2 4

#### Explanation
Type 2 appears twice, Type 4 appears twice. Type 3 appears thrice, Type 1 appears once.

### 2
#### Input
5
5 5 5 6 7

#### Output


#### Explanation
No number appears exactly twice.

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
map, sorting