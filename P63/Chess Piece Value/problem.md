## Title
Chess Piece Value

## Slug
chess-piece-value

## Difficulty
Easy

## Description
A puzzle sets up $n$ pieces in a row. There are 5 types of pieces (Pawn, Knight, Bishop, Rook, Queen), ordered by value. The pieces must be placed in non-decreasing order of value. How many setups are possible?

## Examples

### 1

#### Input
1

#### Output
5

#### Explanation
There are 5 valid sequences of length 1.

### 2

#### Input
2

#### Output
15

#### Explanation
There are 15 valid sorted sequences of length 2 (e.g., aa, ae, ai, ao, au, ee, etc.).

## Input Format
- The input consists of a single integer n, representing the required length/quantity.

## Output Format
- Return a single integer representing the total number of valid sorted sequences.

## Constraints
- 1 ≤ n ≤ 50

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math
