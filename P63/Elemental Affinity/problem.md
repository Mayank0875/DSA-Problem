## Title
Elemental Affinity

## Slug
elemental-affinity

## Difficulty
Easy

## Description
A mage channels $n$ orbs of energy. The orbs come in 5 elements: Earth, Water, Wind, Fire, Void. These elements have a strict cosmological order. A stable channel requires the orbs to be ordered non-decreasingly according to this cosmology. Count the valid channel configurations.

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
