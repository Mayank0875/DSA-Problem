## Title

Dual-Role Players

## Slug

dual-role-players

## Difficulty

Easy

## Description

A team roster lists all player IDs, with some players listed multiple times for different roles. A 'dual-role' player is one whose ID appears exactly twice on the roster. Given the complete roster of IDs, find all dual-role players. Return their IDs in increasing order. If no player has exactly two roles, return an empty list.

## Examples

### 1
#### Input
8
1 2 2 3 3 3 4 4

#### Output
2 4

#### Explanation
2 appears twice, 4 appears twice. 3 appears thrice (not dual-role), 1 appears once.

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