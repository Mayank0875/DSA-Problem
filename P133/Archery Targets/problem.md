## Title
Archery Targets

## Slug
archery-targets

## Difficulty
Medium

## Description
Targets are lined up. An arrow flies through, hitting the fewest targets.

There is a range consisting of $n$ lanes. Each lane is composed of several targets, each having a specific width (integers). The total width of every lane is identical.

You need to shoot a arrow from the start to the end of the range that minimizes the number of targets it hits.

If the arrow passes exactly through the empty space between two targets, it is **not** considered as hitting a target. However, you cannot place the arrow at the very left or the very right of the range.

Given the 2D array `structure` containing the widths of the targets in each lane, return the minimum number of targets hit.

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
We can shoot a arrow at distance 4 from the left.
- Lane 1: 1+2+2=5 (Hit)
- Lane 2: 3+1=4 (Space)
- Lane 3: 1+3=4 (Space)
- Lane 4: 2 (Hit)
- Lane 5: 3+1=4 (Space)
- Lane 6: 1+3=4 (Space)
The arrow hits lanes 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal empty spaces. Any arrow drawn must hit all 3 targets.

## Input Format
- The first line contains an integer $n$, the number of lanes.
- The next $n$ lines each contain space-separated integers representing the widths of the targets in that lane.

## Output Format
- Return a single integer representing the minimum number of targets hit.

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

