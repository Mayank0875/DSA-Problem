## Title
Keyboard Keys

## Slug
keyboard-keys

## Difficulty
Medium

## Description
Rows of keys on a keyboard. A crumb falls between the keys, hitting the fewest keycaps.

There is a keyboard consisting of $n$ rows. Each row is composed of several keys, each having a specific width (integers). The total width of every row is identical.

You need to drop a crumb from the top to the bottom of the keyboard that minimizes the number of keys it lands on.

If the crumb passes exactly through the gap between two keys, it is **not** considered as landing on a key. However, you cannot place the crumb at the very left or the very right of the keyboard.

Given the 2D array `structure` containing the widths of the keys in each row, return the minimum number of keys landed on.

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
We can drop a crumb at distance 4 from the left.
- Row 1: 1+2+2=5 (Land)
- Row 2: 3+1=4 (Gap)
- Row 3: 1+3=4 (Gap)
- Row 4: 2 (Land)
- Row 5: 3+1=4 (Gap)
- Row 6: 1+3=4 (Gap)
The crumb lands on rows 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal gaps. Any crumb drawn must land on all 3 keys.

## Input Format
- The first line contains an integer $n$, the number of rows.
- The next $n$ lines each contain space-separated integers representing the widths of the keys in that row.

## Output Format
- Return a single integer representing the minimum number of keys landed on.

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

