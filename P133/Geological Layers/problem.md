## Title
Geological Layers

## Slug
geological-layers

## Difficulty
Medium

## Description
Rock strata have hard stones and soft soil. A drill wants to go down passing through the fewest hard stones.

There is a ground consisting of $n$ strata. Each stratum is composed of several stones, each having a specific width (integers). The total width of every stratum is identical.

You need to drill a shaft from the surface to the bedrock of the ground that minimizes the number of stones it hits.

If the shaft passes exactly through the soil between two stones, it is **not** considered as hitting a stone. However, you cannot place the shaft at the very west or the very east of the ground.

Given the 2D array `structure` containing the widths of the stones in each stratum, return the minimum number of stones hit.

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
We can drill a shaft at distance 4 from the west.
- Stratum 1: 1+2+2=5 (Hit)
- Stratum 2: 3+1=4 (Soil)
- Stratum 3: 1+3=4 (Soil)
- Stratum 4: 2 (Hit)
- Stratum 5: 3+1=4 (Soil)
- Stratum 6: 1+3=4 (Soil)
The shaft hits strata 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal soils. Any shaft drawn must hit all 3 stones.

## Input Format
- The first line contains an integer $n$, the number of strata.
- The next $n$ lines each contain space-separated integers representing the widths of the stones in that stratum.

## Output Format
- Return a single integer representing the minimum number of stones hit.

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

