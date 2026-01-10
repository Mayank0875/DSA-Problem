## Title
Cell Tower Coverage

## Slug
cell-tower-coverage

## Difficulty
Medium

## Description
A telecom company wants to cover rural villages along a highway. They have tower sites available and need to determine the transmitter strength.

There are $n$ villages and $m$ cell towers positioned at specific coordinates along a highway.

The engineer plans to establish a service range. All cell towers will operate with the same signal range $r$. A cell tower at location $x$ with signal range $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every village must be covered by at least one cell tower.

Your task is to determine the **minimum non-negative integer signal range $r$** required to ensure that all $n$ villages are within the range of at least one cell tower.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
villages are at -2, 2, 4. cell towers are at -3, 0.
With signal range 4:
- cell tower at -3 covers [-7, 1]. Covers village at -2.
- cell tower at 0 covers [-4, 4]. Covers villages at -2, 2, 4.
All villages covered. Minimum signal range is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With signal range 3:
- cell tower at 4 covers [1, 7]. Covers villages 1, 5.
- cell tower at 11 covers [8, 14]. Covers villages 10, 14.
- cell tower at 15 covers [12, 18]. Covers village 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of villages and cell towers.
- The second line contains $n$ integers representing the coordinates of the villages. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the cell towers. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal signal range $r$ required.

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
