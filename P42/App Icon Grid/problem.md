## Title
App Icon Grid

## Slug
app-icon-grid

## Difficulty
Easy

## Description
A mobile OS designer is creating a folder view that displays app icons in a square grid (e.g., 3x3, 4x4). You are given the total number of apps a user wants to group. Calculate the dimension of the largest square grid that can be fully populated by these apps.

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
- A single integer x — the total number of apps available.

## Output Format
- Return single integer — the maximum possible side length r of the square grid that can be built using those apps.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
