## Title
Cinema Seat Pricing

## Slug
cinema-seat-pricing

## Difficulty
Easy

## Description
A row has $n$ seats. There are 5 pricing tiers. Seats are assigned tiers such that prices never decrease as you move from the edge to the center (simplified linear model). How many pricing layouts are possible?

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
