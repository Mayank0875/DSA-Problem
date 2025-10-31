## Title

Duet Note Identifier

## Slug

duet-note-identifier

## Difficulty

Easy

## Description

A musicologist is analyzing a composition, represented as a list of musical notes (integers). A 'duet note' is a note that is played exactly twice in the piece. Given the list of notes, find all duet notes. Return them in increasing order. If no note is played exactly twice, return an empty list.

## Examples

### 1
#### Input
8
1 2 2 3 3 3 4 4

#### Output
2 4

#### Explanation
2 appears twice, 4 appears twice. 3 appears thrice (not a duet note), 1 appears once.

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