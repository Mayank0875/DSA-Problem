## Title
Customer Loyalty Tiers

## Slug
customer-loyalty-tiers

## Difficulty
Easy

## Description
A rewards program tracks a customer's status over $n$ months. There are 5 tiers: Bronze, Silver, Gold, Platinum, Diamond. A customer's tier can never drop, only stay the same or increase. How many status progression histories are possible over $n$ months?

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
