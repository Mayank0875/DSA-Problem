## Title

Largest Skyline Banner

## Slug

largest-skyline-banner

## Difficulty

Medium

## Description

Imagine a cityscape represented by a series of adjacent rectangular buildings of varying heights but uniform width (width = 1 unit). 
You are tasked with finding the maximum possible rectangular area for a banner that can be placed perfectly flat against the skyline, aligned with the building bases. The banner must fit entirely within the bounds defined by the building heights. You are given the heights of n adjacent buildings. Determine the largest possible area for such a banner.

## Examples

### 1

#### Input

7
[6, 2, 5, 4, 5, 1, 6]

#### Output

12

#### Explanation

The largest rectangular banner has a height of 4 and spans across buildings with heights [5, 4, 5]. The width is 3 units (from index 2 to 4). Area = height * width = 4 * 3 = 12.

### 2

#### Input

4
[2, 1, 5, 6]

#### Output

10

#### Explanation

The largest rectangle has height 5 and spans buildings with heights [5, 6]. Width = 2. Area = 5 * 2 = 10.
  

## Input Format  

- The first line contains a single integer n, the number of buildings.
- The second line contains n space-separated integers, representing the heights of the buildings from left to right.

## Output Format  

- Return a single integer representing the maximum possible rectangular banner area.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ height ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array