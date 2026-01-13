## Title
City Skyline Gap

## Slug
city-skyline-gap

## Difficulty
Medium

## Description
A city has multiple streets with buildings. You want to see the sunset through a gap that is blocked by the fewest buildings.

There is a city block consisting of $n$ streets. Each street is composed of several buildings, each having a specific width (integers). The total width of every street is identical.

You need to find a line of sight from the front to the back of the city block that minimizes the number of buildings it is blocked by.

If the line of sight passes exactly through the alley between two buildings, it is **not** considered as being blocked by a building. However, you cannot place the line of sight at the very west limit or the very east limit of the city block.

Given the 2D array `structure` containing the widths of the buildings in each street, return the minimum number of buildings blocked.

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
We can find a line of sight at distance 4 from the west limit.
- Street 1: 1+2+2=5 (Blocked)
- Street 2: 3+1=4 (Alley)
- Street 3: 1+3=4 (Alley)
- Street 4: 2 (Blocked)
- Street 5: 3+1=4 (Alley)
- Street 6: 1+3=4 (Alley)
The line of sight is blocked by streets 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal alleys. Any line of sight drawn must be blocked by all 3 buildings.

## Input Format
- The first line contains an integer $n$, the number of streets.
- The next $n$ lines each contain space-separated integers representing the widths of the buildings in that street.

## Output Format
- Return a single integer representing the minimum number of buildings blocked.

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

