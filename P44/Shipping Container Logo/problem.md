## Title
Shipping Container Logo

## Slug
shipping-container-logo

## Difficulty
Medium

## Description
A cargo ship has a row of container stacks of different heights. The shipping company wants to paint a large rectangular logo across the side of these stacks. The logo cannot hover in the air; it must be painted on the containers. Find the largest rectangular area available for the logo.

## Examples

### 1

#### Input
7
[6, 2, 5, 4, 5, 1, 6]

#### Output
12

#### Explanation
The largest rectangular area has a height of 4 and spans across elements with heights [5, 4, 5]. The width is 3 units (from index 2 to 4). Area = height * width = 4 * 3 = 12.

### 2

#### Input
4
[2, 1, 5, 6]

#### Output
10

#### Explanation
The largest rectangle has height 5 and spans elements with heights [5, 6]. Width = 2. Area = 5 * 2 = 10.

## Input Format
- The first line contains a single integer n, the number of elements.
- The second line contains n space-separated integers, representing the heights/values of the elements from left to right.

## Output Format
- Return a single integer representing the maximum possible rectangular area.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ height ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, array
