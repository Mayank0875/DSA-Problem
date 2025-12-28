## Title
Wildlife Migration

## Slug
wildlife-migration

## Difficulty
Medium

## Description
Birds stop at various sanctuaries. Each sanctuary is open for migration during specific weeks.

The map shows list of sanctuaries, each defined by a open week and an close week, represented as a pair `[open, close]`.

Birds fly north. They must leave a sanctuary strictly before the opening week of the next sanctuary to catch the wind currents. Specifically, to transition from sanctuary `[a, b]` to a subsequent sanctuary `[c, d]`, the close of the first sanctuary must be **strictly less than** the open of the second sanctuary (i.e., `b < c`).

You can select sanctuaries in any order you like to form a valid route. Your goal is to determine the maximum number of sanctuaries that can be included in a single route.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest route is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The sanctuaries can be reordered to form the route `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available sanctuaries.
- The next `n` lines each contain two integers, representing the `open` and `close` of an sanctuary.

## Output Format
- Return a single integer representing the maximum length of the route.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ open < close ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
