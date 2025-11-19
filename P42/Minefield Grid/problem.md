## Title
Minefield Grid

## Slug
minefield-grid

## Difficulty
Easy

## Description
You are programming a minesweeper clone. The game board must be a square grid. Given the total number of safe tiles the map generator can produce, calculate the side length of the largest square board that can be created.

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
- A single integer x — the total number of tiles available.

## Output Format
- Return single integer — the maximum possible side length r of the square board that can be built using those tiles.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
