## Title
Billboard Slats

## Slug
billboard-slats

## Difficulty
Medium

## Description
A rotating billboard has slats. You need to cut the billboard vertically, damaging the fewest image slats.

There is a billboard consisting of $n$ sections. Each section is composed of several slats, each having a specific width (integers). The total width of every section is identical.

You need to cut a line from the top to the bottom of the billboard that minimizes the number of slats it damages.

If the line passes exactly through the joint between two slats, it is **not** considered as damaging a slat. However, you cannot place the line at the very left or the very right of the billboard.

Given the 2D array `structure` containing the widths of the slats in each section, return the minimum number of slats damaged.

## Examples

### 1

#### Input
6
1 2 2 1
3 1 2
1 3 2
2 4
3 1 2
1 3 1 1

#### Output
2

#### Explanation
The total width is 6.
We can cut a line at distance 4 from the left.
- Section 1: 1+2+2=5 (Damage)
- Section 2: 3+1=4 (Joint)
- Section 3: 1+3=4 (Joint)
- Section 4: 2 (Damage)
- Section 5: 3+1=4 (Joint)
- Section 6: 1+3=4 (Joint)
The line damages sections 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal joints. Any line drawn must damage all 3 slats.

## Input Format
- The first line contains an integer $n$, the number of sections.
- The next $n$ lines each contain space-separated integers representing the widths of the slats in that section.

## Output Format
- Return a single integer representing the minimum number of slats damaged.

## Constraints
- 1 ≤ n ≤ 10^4
- 1 <= structure[i].length <= 10^4
- The sum of elements in each row is the same.
- 1 <= structure[i][j] <= 2^31 - 1

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, prefix-sum

