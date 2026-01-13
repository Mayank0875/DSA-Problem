## Title
Server Rack Airflow

## Slug
server-rack-airflow

## Difficulty
Medium

## Description
Servers block airflow. You need to position a vent to blow air through the rack blocked by the fewest servers.

There is a rack consisting of $n$ shelves. Each shelf is composed of several servers, each having a specific width (integers). The total width of every shelf is identical.

You need to position a vent from the front to the back of the rack that minimizes the number of servers it is blocked by.

If the vent passes exactly through the vent hole between two servers, it is **not** considered as being blocked by a server. However, you cannot place the vent at the very left or the very right of the rack.

Given the 2D array `structure` containing the widths of the servers in each shelf, return the minimum number of servers blocked.

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
We can position a vent at distance 4 from the left.
- Shelf 1: 1+2+2=5 (Blocked)
- Shelf 2: 3+1=4 (Vent hole)
- Shelf 3: 1+3=4 (Vent hole)
- Shelf 4: 2 (Blocked)
- Shelf 5: 3+1=4 (Vent hole)
- Shelf 6: 1+3=4 (Vent hole)
The vent is blocked by shelves 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal vent holes. Any vent drawn must be blocked by all 3 servers.

## Input Format
- The first line contains an integer $n$, the number of shelves.
- The next $n$ lines each contain space-separated integers representing the widths of the servers in that shelf.

## Output Format
- Return a single integer representing the minimum number of servers blocked.

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

