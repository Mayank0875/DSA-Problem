## Title
Card Game Patience

## Slug
card-game-patience

## Difficulty
Easy

## Description
You are playing a solitaire game where cards must be dealt into a square grid face down. You have a deck with a specific number of cards. Determine the side length of the largest square grid you can deal using the cards in your hand.

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
- A single integer x — the total number of cards available.

## Output Format
- Return single integer — the maximum possible side length r of the square grid that can be built using those cards.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
