## Title
Railway Track Switching

## Slug
railway-track-switching

## Difficulty
Medium

## Description
Two parallel railway tracks need crossover switches to divert trains in case of track failure.

Two parallel tracks, Express Line and Local Line, each contain n signal posts arranged in a line.
Express Line has an array `a` representing the signal frequency of each post.
Local Line has an array `b` representing the signal frequency of each post.

Inside each track, adjacent signal posts are already connected by internal rails.

You must establish inter-track switches connecting some signal posts of Express Line to some signal posts of Local Line.

The cost to create a switch between post i of Express Line and post j of Local Line is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single post is removed (from either Express Line or Local Line).
If one post fails and disappears along with all its connections, the remaining signal posts must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of signal posts:
1. post 1 from Express Line with post 2 from Local Line: cost |1-4| = 3.
2. post 3 from Express Line with post 2 from Local Line: cost |1-4| = 3.
3. post 2 from Express Line with post 1 from Local Line: cost |10-20| = 10.
4. post 2 from Express Line with post 3 from Local Line: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first post of Express Line with the first of Local Line, and the last post of Express Line with the last of Local Line, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of signal posts in each track.
- The second line contains n integers representing the signal frequencys of Express Line.
- The third line contains n integers representing the signal frequencys of Local Line.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
