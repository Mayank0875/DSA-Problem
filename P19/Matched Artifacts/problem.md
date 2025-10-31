## Title

Matched Artifacts

## Slug

matched-artifacts

## Difficulty

Easy

## Description

An archaeologist has a list of artifact IDs from an excavation. A 'matched artifact' is an item that is one of a pair, meaning its ID appears exactly twice in the collection. Given the list of IDs, find all matched artifacts. Return their IDs in increasing order. If no artifact is part of a pair, return an empty list.

## Examples

### 1
#### Input
8
1 2 2 3 3 3 4 4

#### Output
2 4

#### Explanation
2 appears twice, 4 appears twice. 3 appears thrice (not matched), 1 appears once.

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