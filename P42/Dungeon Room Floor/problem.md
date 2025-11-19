## Title
Dungeon Room Floor

## Slug
dungeon-room-floor

## Difficulty
Easy

## Description
A level designer is creating a square room in a dungeon crawler game. The floor is made of square stone slabs. Given the total number of slab assets allowed for the room, find the side length of the largest square room that can be tiled.

## Examples

### 1

#### Input
10

#### Output
3

#### Explanation
3² = 9 ≤ 10, 4² = 16 > 10

### 2

#### Input
25

#### Output
5

#### Explanation
5² = 25 ≤ 25, 6² = 36 > 25

## Input Format
- A single integer x — the total number of slabs available.

## Output Format
- Return single integer — the maximum possible side length r of the square room that can be built using those slabs.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
