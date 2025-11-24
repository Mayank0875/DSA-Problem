## Title
Geological Layering

## Slug
geological-layering

## Difficulty
Easy

## Description
A core sample contains $n$ distinct layers of sediment. There are 5 types of sediment, which settle in a specific density order. Heavier sediments are never found above lighter ones in this region. How many valid layer sequences can a core sample of size $n$ have?

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
