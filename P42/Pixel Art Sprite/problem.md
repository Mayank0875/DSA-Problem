## Title
Pixel Art Sprite

## Slug
pixel-art-sprite

## Difficulty
Easy

## Description
A pixel artist is drawing a character sprite that must fit within a square canvas. Given the total number of colored pixels they plan to use for the base, determine the width of the largest square canvas that can be fully filled with this number of pixels.

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
- A single integer x — the total number of pixels available.

## Output Format
- Return single integer — the maximum possible side length r of the square canvas that can be built using those pixels.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
