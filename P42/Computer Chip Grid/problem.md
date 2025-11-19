## Title
Computer Chip Grid

## Slug
computer-chip-grid

## Difficulty
Easy

## Description
In semiconductor manufacturing, identical logic gates are arranged in a square grid on a silicon die. You are given the total number of functioning logic gates available for a single chip. Your task is to find the dimension (number of gates per side) of the largest square grid that can be formed.

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
- A single integer x — the total number of logic gates available.

## Output Format
- Return single integer — the maximum possible side length r of the square chip grid that can be built using those logic gates.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
