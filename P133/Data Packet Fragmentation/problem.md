## Title
Data Packet Fragmentation

## Slug
data-packet-fragmentation

## Difficulty
Medium

## Description
Data streams are sent in packets. You need to insert a synchronization marker that splits the fewest packets.

There is a data stream consisting of $n$ channels. Each channel is composed of several packets, each having a specific size (integers). The total size of every channel is identical.

You need to insert a marker from the start to the end of the data stream that minimizes the number of packets it splits.

If the marker passes exactly through the gap between two packets, it is **not** considered as splitting a packet. However, you cannot place the marker at the very beginning or the very termination of the data stream.

Given the 2D array `structure` containing the sizes of the packets in each channel, return the minimum number of packets split.

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
The total size is 6.
We can insert a marker at distance 4 from the beginning.
- Channel 1: 1+2+2=5 (Split)
- Channel 2: 3+1=4 (Gap)
- Channel 3: 1+3=4 (Gap)
- Channel 4: 2 (Split)
- Channel 5: 3+1=4 (Gap)
- Channel 6: 1+3=4 (Gap)
The marker splits channels 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal gaps. Any marker drawn must split all 3 packets.

## Input Format
- The first line contains an integer $n$, the number of channels.
- The next $n$ lines each contain space-separated integers representing the sizes of the packets in that channel.

## Output Format
- Return a single integer representing the minimum number of packets split.

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

