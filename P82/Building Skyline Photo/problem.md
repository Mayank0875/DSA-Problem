## Title
Building Skyline Photo

## Slug
building-skyline-photo

## Difficulty
Easy

## Description
A photographer takes a panoramic shot of n buildings. They want to crop the photo to show a 'rising skyline' effect, keeping buildings that are taller than the one to their left.

You have the heights of n buildings in a row.
A rising skyline consists of buildings where each building is strictly taller than the previously selected building to its left.

You must crop the panorama to find the longest possible rising skyline. You can skip any number of buildings to form the sequence, but you must maintain the original left-to-right order of the selected buildings. Calculate the maximum number of buildings that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest rising skylines (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 building.

## Input Format
- The first line contains an integer n: the number of buildings.
- The second line contains n integers x_1, x_2 ... x_n: the height of each building in order.

## Output Format
- Return one integer: the length of the longest valid rising skyline.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
