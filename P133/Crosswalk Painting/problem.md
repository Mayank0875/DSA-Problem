## Title
Crosswalk Painting

## Slug
crosswalk-painting

## Difficulty
Medium

## Description
A road has existing paint lines. A new utility line must be painted across, crossing the fewest existing paint stripes.

There is a road consisting of $n$ lanes. Each lane is composed of several stripes, each having a specific length (integers). The total length of every lane is identical.

You need to paint a utility line from the curb 1 to the curb 2 of the road that minimizes the number of stripes it overlaps.

If the utility line passes exactly through the asphalt between two stripes, it is **not** considered as overlapping a stripe. However, you cannot place the utility line at the very start or the very end of the road.

Given the 2D array `structure` containing the lengths of the stripes in each lane, return the minimum number of stripes overlapped.

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
The total length is 6.
We can paint a utility line at distance 4 from the start.
- Lane 1: 1+2+2=5 (Overlap)
- Lane 2: 3+1=4 (Asphalt)
- Lane 3: 1+3=4 (Asphalt)
- Lane 4: 2 (Overlap)
- Lane 5: 3+1=4 (Asphalt)
- Lane 6: 1+3=4 (Asphalt)
The utility line overlaps lanes 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal asphalts. Any utility line drawn must overlap all 3 stripes.

## Input Format
- The first line contains an integer $n$, the number of lanes.
- The next $n$ lines each contain space-separated integers representing the lengths of the stripes in that lane.

## Output Format
- Return a single integer representing the minimum number of stripes overlapped.

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

