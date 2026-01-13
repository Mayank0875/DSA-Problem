## Title
City Parade Route

## Slug
city-parade-route

## Difficulty
Medium

## Description
Crowds line the streets. A float moves down the center, bumping into the fewest crowd barriers.

There is a route consisting of $n$ blocks. Each block is composed of several barriers, each having a specific length (integers). The total length of every block is identical.

You need to drive a float from the start to the end of the route that minimizes the number of barriers it bumps.

If the float passes exactly through the opening between two barriers, it is **not** considered as bumping a barrier. However, you cannot place the float at the very left or the very right of the route.

Given the 2D array `structure` containing the lengths of the barriers in each block, return the minimum number of barriers bumped.

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
We can drive a float at distance 4 from the left.
- Block 1: 1+2+2=5 (Bump)
- Block 2: 3+1=4 (Opening)
- Block 3: 1+3=4 (Opening)
- Block 4: 2 (Bump)
- Block 5: 3+1=4 (Opening)
- Block 6: 1+3=4 (Opening)
The float bumps blocks 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal openings. Any float drawn must bump all 3 barriers.

## Input Format
- The first line contains an integer $n$, the number of blocks.
- The next $n$ lines each contain space-separated integers representing the lengths of the barriers in that block.

## Output Format
- Return a single integer representing the minimum number of barriers bumped.

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

