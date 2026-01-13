## Title

Brick Wall Cut

## Slug

brick-wall-cut

## Difficulty

Medium

## Description

There is a rectangular brick wall in front of you with $n$ rows of bricks. The $i$-th row has some number of bricks, each of the same height (one unit) but potentially different widths. The total width of each row is the same.

You need to draw a vertical line from the top to the bottom of the wall and cross the minimum number of bricks. If the line passes through the edge between two bricks, it is not considered as crossing a brick. However, you cannot draw the line along the two vertical edges of the wall (the far left or far right).

Given the 2D array `wall` containing the widths of bricks in each row, return the minimum number of crossed bricks.

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
We can draw a line at distance 4 from the left.
- Row 1: 1+2+2=5 (Cut)
- Row 2: 3+1=4 (Edge)
- Row 3: 1+3=4 (Edge)
- Row 4: 2 (Cut)
- Row 5: 3+1=4 (Edge)
- Row 6: 1+3=4 (Edge)
The line crosses rows 1 and 4. Total crossed: 2.
    
### 2

#### Input

3
1
1
1

#### Output

3

#### Explanation

There are no internal edges. Any line drawn must cross all 3 bricks.

## Input Format  

- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the bricks in that row.

## Output Format  

- Return a single integer representing the minimum number of crossed bricks.
  

## Constraints  

- 1 ≤ n ≤ 1e4
- 1 <= wall[i].length <= 104
- 1 <= sum(wall[i].length) <= 2 * 104
- sum(wall[i]) is the same for each row i.
- 1 <= wall[i][j] <= 231 - 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, hash-table

## Company
grab