## Title
Microscope Grid Count

## Slug
microscope-grid-count

## Difficulty
Easy

## Description
A biologist is counting cells placed on a square grid slide. To ensure statistical significance, they define a square region of interest. Given the total number of cells visible, calculate the side length of the largest square grid of cells that can be formed if they were packed tightly.

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
- A single integer x — the total number of cells available.

## Output Format
- Return single integer — the maximum possible side length r of the square grid that can be built using those cells.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
