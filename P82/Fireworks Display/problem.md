## Title
Fireworks Display

## Slug
fireworks-display

## Difficulty
Easy

## Description
A show has n fireworks. The finale requires a sequence of strictly increasing explosion sizes.

You have explosion radii for n fireworks.
A finale sequence consists of fireworks where the radius is strictly larger than the previous one.

You must plan the show to find the longest possible grand finale. You can skip any number of fireworks to form the sequence, but you must maintain the original launch order order of the selected fireworks. Calculate the maximum number of fireworks that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest grand finales (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 firework.

## Input Format
- The first line contains an integer n: the number of fireworks.
- The second line contains n integers x_1, x_2 ... x_n: the radius of each firework in order.

## Output Format
- Return one integer: the length of the longest valid grand finale.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
