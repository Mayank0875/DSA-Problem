## Title
Stone Henge

## Slug
stone-henge

## Difficulty
Medium

## Description
Stones are arranged in circles (rows). A sunbeam shines through, hitting the fewest stones.

There is a monument consisting of $n$ circles. Each circle is composed of several stones, each having a specific arc length (integers). The total arc length of every circle is identical.

You need to shine a beam from the outside to the center of the monument that minimizes the number of stones it strikes.

If the beam passes exactly through the gap between two stones, it is **not** considered as striking a stone. However, you cannot place the beam at the very start or the very end of the monument.

Given the 2D array `structure` containing the arc lengths of the stones in each circle, return the minimum number of stones struck.

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
The total arc length is 6.
We can shine a beam at distance 4 from the start.
- Circle 1: 1+2+2=5 (Strike)
- Circle 2: 3+1=4 (Gap)
- Circle 3: 1+3=4 (Gap)
- Circle 4: 2 (Strike)
- Circle 5: 3+1=4 (Gap)
- Circle 6: 1+3=4 (Gap)
The beam strikes circles 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal gaps. Any beam drawn must strike all 3 stones.

## Input Format
- The first line contains an integer $n$, the number of circles.
- The next $n$ lines each contain space-separated integers representing the arc lengths of the stones in that circle.

## Output Format
- Return a single integer representing the minimum number of stones struck.

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

