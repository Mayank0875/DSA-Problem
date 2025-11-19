## Title
LED Matrix Panel

## Slug
led-matrix-panel

## Difficulty
Easy

## Description
An electronics hobbyist has a bag of LEDs and wants to solder them into a square matrix display. Given the total number of LEDs available, find the number of LEDs that will make up the width of the largest possible square matrix.

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
- A single integer x — the total number of LEDs available.

## Output Format
- Return single integer — the maximum possible side length r of the square matrix that can be built using those LEDs.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
