## Title
Solar Panel Shadows

## Slug
solar-panel-shadows

## Difficulty
Medium

## Description
Rows of panels cast shadows. You want to lay a cable that stays in the sun (gaps) and crosses the fewest shadows.

There is a field consisting of $n$ arrays. Each array is composed of several shadows, each having a specific width (integers). The total width of every array is identical.

You need to lay a cable from the north to the south of the field that minimizes the number of shadows it enters.

If the cable passes exactly through the sunlight between two shadows, it is **not** considered as entering a shadow. However, you cannot place the cable at the very west or the very east of the field.

Given the 2D array `structure` containing the widths of the shadows in each array, return the minimum number of shadows entered.

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
We can lay a cable at distance 4 from the west.
- Array 1: 1+2+2=5 (Enter)
- Array 2: 3+1=4 (Sunlight)
- Array 3: 1+3=4 (Sunlight)
- Array 4: 2 (Enter)
- Array 5: 3+1=4 (Sunlight)
- Array 6: 1+3=4 (Sunlight)
The cable enters arrays 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal sunlights. Any cable drawn must enter all 3 shadows.

## Input Format
- The first line contains an integer $n$, the number of arrays.
- The next $n$ lines each contain space-separated integers representing the widths of the shadows in that array.

## Output Format
- Return a single integer representing the minimum number of shadows entered.

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

