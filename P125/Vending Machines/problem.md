## Title
Vending Machines

## Slug
vending-machines

## Difficulty
Medium

## Description
Thirsty students in classrooms along a hallway need access to vending machines.

There are $n$ classrooms and $m$ machines positioned at specific coordinates along a hallway.

The principal plans to establish a service range. All machines will operate with the same walking distance $r$. A machine at location $x$ with walking distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every classroom must be covered by at least one machine.

Your task is to determine the **minimum non-negative integer walking distance $r$** required to ensure that all $n$ classrooms are within the range of at least one machine.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
classrooms are at -2, 2, 4. machines are at -3, 0.
With walking distance 4:
- machine at -3 covers [-7, 1]. Covers classroom at -2.
- machine at 0 covers [-4, 4]. Covers classrooms at -2, 2, 4.
All classrooms covered. Minimum walking distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With walking distance 3:
- machine at 4 covers [1, 7]. Covers classrooms 1, 5.
- machine at 11 covers [8, 14]. Covers classrooms 10, 14.
- machine at 15 covers [12, 18]. Covers classroom 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of classrooms and machines.
- The second line contains $n$ integers representing the coordinates of the classrooms. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the machines. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal walking distance $r$ required.

## Constraints
- 1 ≤ n, m ≤ 10^5
- -10^9 ≤ coordinates ≤ 10^9
- The input arrays are sorted in non-decreasing order.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, two-pointers, array, math
