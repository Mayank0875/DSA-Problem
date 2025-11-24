## Title
Coffee Roast Selection

## Slug
coffee-roast-selection

## Difficulty
Easy

## Description
A coffee subscription box sends $n$ bags of coffee. There are 5 roast levels: Blonde, Medium, City, French, and Italian. Subscribers can choose their box, but the roasts must be packed in non-decreasing intensity order. How many different box combinations can be ordered?

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
