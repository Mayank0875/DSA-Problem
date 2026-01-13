## Title
Fence Picket Alignment

## Slug
fence-picket-alignment

## Difficulty
Medium

## Description
A fence has horizontal rails with pickets nailed on. You want to saw through the fence hitting the fewest pickets.

There is a fence consisting of $n$ rails. Each rail is composed of several pickets, each having a specific width (integers). The total width of every rail is identical.

You need to saw a line from the top to the bottom of the fence that minimizes the number of pickets it saws through.

If the line passes exactly through the gap between two pickets, it is **not** considered as sawing through a picket. However, you cannot place the line at the very left post or the very right post of the fence.

Given the 2D array `structure` containing the widths of the pickets in each rail, return the minimum number of pickets sawed.

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
We can saw a line at distance 4 from the left post.
- Rail 1: 1+2+2=5 (Saw)
- Rail 2: 3+1=4 (Gap)
- Rail 3: 1+3=4 (Gap)
- Rail 4: 2 (Saw)
- Rail 5: 3+1=4 (Gap)
- Rail 6: 1+3=4 (Gap)
The line saws through rails 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal gaps. Any line drawn must saw through all 3 pickets.

## Input Format
- The first line contains an integer $n$, the number of rails.
- The next $n$ lines each contain space-separated integers representing the widths of the pickets in that rail.

## Output Format
- Return a single integer representing the minimum number of pickets sawed.

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

