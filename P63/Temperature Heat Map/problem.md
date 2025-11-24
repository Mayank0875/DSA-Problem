## Title
Temperature Heat Map

## Slug
temperature-heat-map

## Difficulty
Easy

## Description
A sensor array has $n$ points arranged linearly. It detects heat levels 1 to 5. In a heat source experiment, the temperature must be non-decreasing as you move closer to the source (along the array). How many valid heat map patterns can be recorded?

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
