## Title
Piano Key Alignment

## Slug
piano-key-alignment

## Difficulty
Medium

## Description
A player piano roll has holes. You want to draw a line that passes over the fewest holes.

There is a roll consisting of $n$ measures. Each measure is composed of several holes, each having a specific duration (integers). The total duration of every measure is identical.

You need to draw a line from the top to the bottom of the roll that minimizes the number of holes it crosses.

If the line passes exactly through the paper between two holes, it is **not** considered as crossing a hole. However, you cannot place the line at the very start or the very end of the roll.

Given the 2D array `structure` containing the durations of the holes in each measure, return the minimum number of holes crossed.

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
The total duration is 6.
We can draw a line at distance 4 from the start.
- Measure 1: 1+2+2=5 (Cross)
- Measure 2: 3+1=4 (Paper)
- Measure 3: 1+3=4 (Paper)
- Measure 4: 2 (Cross)
- Measure 5: 3+1=4 (Paper)
- Measure 6: 1+3=4 (Paper)
The line crosses measures 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal papers. Any line drawn must cross all 3 holes.

## Input Format
- The first line contains an integer $n$, the number of measures.
- The next $n$ lines each contain space-separated integers representing the durations of the holes in that measure.

## Output Format
- Return a single integer representing the minimum number of holes crossed.

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

