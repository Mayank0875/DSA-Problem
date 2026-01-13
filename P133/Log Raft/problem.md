## Title
Log Raft

## Slug
log-raft

## Difficulty
Medium

## Description
Logs are tied in a raft. A spear is thrown, hitting the fewest logs.

There is a raft consisting of $n$ layers. Each layer is composed of several logs, each having a specific diameter (integers). The total diameter of every layer is identical.

You need to throw a spear from the top to the bottom of the raft that minimizes the number of logs it pierces.

If the spear passes exactly through the gap between two logs, it is **not** considered as piercing a log. However, you cannot place the spear at the very left or the very right of the raft.

Given the 2D array `structure` containing the diameters of the logs in each layer, return the minimum number of logs pierced.

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
The total diameter is 6.
We can throw a spear at distance 4 from the left.
- Layer 1: 1+2+2=5 (Pierce)
- Layer 2: 3+1=4 (Gap)
- Layer 3: 1+3=4 (Gap)
- Layer 4: 2 (Pierce)
- Layer 5: 3+1=4 (Gap)
- Layer 6: 1+3=4 (Gap)
The spear pierces layers 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal gaps. Any spear drawn must pierce all 3 logs.

## Input Format
- The first line contains an integer $n$, the number of layers.
- The next $n$ lines each contain space-separated integers representing the diameters of the logs in that layer.

## Output Format
- Return a single integer representing the minimum number of logs pierced.

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

