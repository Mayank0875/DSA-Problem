## Title
Cinema Screen Projection

## Slug
cinema-screen-projection

## Difficulty
Medium

## Description
An outdoor cinema is projecting a movie onto a ruined wall. The wall consists of several adjacent broken sections of different heights. The projected image must be a perfect rectangle. To maximize the viewing experience, you want to find the largest rectangular area that fits on the surviving wall sections. Given the heights of the wall sections, calculate this maximum area.

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
