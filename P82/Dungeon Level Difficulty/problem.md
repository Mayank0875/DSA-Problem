## Title
Dungeon Level Difficulty

## Slug
dungeon-level-difficulty

## Difficulty
Easy

## Description
A game generates n dungeon rooms. The difficulty must strictly increase as the player progresses.

You have difficulty scores for n rooms.
A valid progression consists of rooms where difficulty is strictly higher than the previous room.

You must generate dungeon to find the longest possible level progression. You can skip any number of rooms to form the sequence, but you must maintain the original generation order order of the selected rooms. Calculate the maximum number of rooms that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest level progressions (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 room.

## Input Format
- The first line contains an integer n: the number of rooms.
- The second line contains n integers x_1, x_2 ... x_n: the difficulty of each room in order.

## Output Format
- Return one integer: the length of the longest valid level progression.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
