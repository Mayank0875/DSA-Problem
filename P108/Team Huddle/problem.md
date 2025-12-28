## Title
Team Huddle

## Slug
team-huddle

## Difficulty
Easy

## Description
Players in a circle break the huddle and rotate positions for the next drill.

The circle is represented by an array. The drill setup rotates the players $k$ positions to the right. A rotation to the right means the last player moves to the first position, and all other players shift one spot to the right. This process happens $k$ times.

Your task is to determine the final arrangement of the players in the circle. You must achieve this efficiently, ideally modifying the structure in-place.

## Examples

### 1

#### Input
7 3
1 2 3 4 5 6 7

#### Output
5 6 7 1 2 3 4

#### Explanation
Initial: `[1, 2, 3, 4, 5, 6, 7]`
Rotate 1: `[7, 1, 2, 3, 4, 5, 6]`
Rotate 2: `[6, 7, 1, 2, 3, 4, 5]`
Rotate 3: `[5, 6, 7, 1, 2, 3, 4]`

### 2

#### Input
4 2
-1 -100 3 99

#### Output
3 99 -1 -100

#### Explanation
Rotate 1: `[99, -1, -100, 3]`
Rotate 2: `[3, 99, -1, -100]`

## Input Format
- The first line contains two integers, $n$ and $k$, the number of players and the rotation count.
- The second line contains $n$ space-separated integers representing the players.

## Output Format
- Return the array containing the $n$ integers in their new order, separated by spaces.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ k ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, math
