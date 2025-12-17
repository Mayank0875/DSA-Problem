## Title
The Mosaic Floor Project

## Slug
mosaic-floor-project

## Difficulty
Easy

## Description
An interior designer is working on a restoration project for a grand hall. The design calls for a specific section of the floor to be covered by exactly three square ceramic tiles. The warehouse has a large collection of spare square tiles with various side lengths. The designer needs to fill a specific area on the floor plan exactly. You must determine if there are three distinct tiles in the inventory whose combined area equals the target area needed to complete the design.

Your task is to determine whether it is possible to choose three distinct tiles (at indices i < j < k) such that:

    side_i^2 + side_j^2 + side_k^2 = total_area

If it is possible, print YES; otherwise, print NO.

## Examples

### 1
#### Input
5
1 2 2 3 4
9

#### Output
YES

#### Explanation
1^2 + 2^2 + 2^2 = 1 + 4 + 4 = 9.

### 2
#### Input
4
3 3 3 3
20

#### Output
NO

#### Explanation
Every square is 9; any sum of three squares is 27 which is not 20.

## Input Format
- First line: integer n — the number of tiles.
- Second line: n space-separated integers a1 a2 ... an — the side lengths (can be negative, zero, or positive).
- Third line: integer target — the target sum.

## Output Format
- Return true (YES) if there exist indices i < j < k with a[i]^2 + a[j]^2 + a[k]^2 = target, otherwise return false (NO).

## Constraints
- 3 ≤ n ≤ 2000
- -10^6 ≤ ai ≤ 10^6
- 0 ≤ target ≤ 3×10^12

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
two-pointers, sorting, array, maths
