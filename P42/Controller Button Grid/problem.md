## Title
Controller Button Grid

## Slug
controller-button-grid

## Difficulty
Easy

## Description
A hardware designer is creating a custom MIDI controller with a square grid of buttons. You are given the total inventory of switch components. Calculate the width (in buttons) of the largest square grid that can be built.

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
- A single integer x — the total number of switches available.

## Output Format
- Return single integer — the maximum possible side length r of the square grid that can be built using those switches.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
