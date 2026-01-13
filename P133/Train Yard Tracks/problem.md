## Title
Train Yard Tracks

## Slug
train-yard-tracks

## Difficulty
Medium

## Description
Trains are parked on parallel tracks. A worker needs to cross the yard climbing over the fewest trains.

There is a yard consisting of $n$ tracks. Each track is composed of several trains, each having a specific length (integers). The total length of every track is identical.

You need to cross a path from the north to the south of the yard that minimizes the number of trains it climbs.

If the path passes exactly through the gap between two trains, it is **not** considered as climbing a train. However, you cannot place the path at the very west or the very east of the yard.

Given the 2D array `structure` containing the lengths of the trains in each track, return the minimum number of trains climbed.

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
The total length is 6.
We can cross a path at distance 4 from the west.
- Track 1: 1+2+2=5 (Climb)
- Track 2: 3+1=4 (Gap)
- Track 3: 1+3=4 (Gap)
- Track 4: 2 (Climb)
- Track 5: 3+1=4 (Gap)
- Track 6: 1+3=4 (Gap)
The path climbs tracks 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal gaps. Any path drawn must climb all 3 trains.

## Input Format
- The first line contains an integer $n$, the number of tracks.
- The next $n$ lines each contain space-separated integers representing the lengths of the trains in that track.

## Output Format
- Return a single integer representing the minimum number of trains climbed.

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

