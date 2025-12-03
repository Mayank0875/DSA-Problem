## Title
Video Game Checkpoints

## Slug
video-game-checkpoints

## Difficulty
Medium

## Description
A level designer connects two parallel paths with shortcuts to prevent players getting stuck.

Two parallel paths, Forest Path and Cave Path, each contain n checkpoints arranged in a line.
Forest Path has an array `a` representing the difficulty level of each checkpoint.
Cave Path has an array `b` representing the difficulty level of each checkpoint.

Inside each path, adjacent checkpoints are already connected by internal trails.

You must establish inter-path shortcuts connecting some checkpoints of Forest Path to some checkpoints of Cave Path.

The cost to create a shortcut between checkpoint i of Forest Path and checkpoint j of Cave Path is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single checkpoint is removed (from either Forest Path or Cave Path).
If one checkpoint fails and disappears along with all its connections, the remaining checkpoints must still form a single connected network.

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
It's optimal to connect four pairs of checkpoints:
1. checkpoint 1 from Forest Path with checkpoint 2 from Cave Path: cost |1-4| = 3.
2. checkpoint 3 from Forest Path with checkpoint 2 from Cave Path: cost |1-4| = 3.
3. checkpoint 2 from Forest Path with checkpoint 1 from Cave Path: cost |10-20| = 10.
4. checkpoint 2 from Forest Path with checkpoint 3 from Cave Path: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first checkpoint of Forest Path with the first of Cave Path, and the last checkpoint of Forest Path with the last of Cave Path, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of checkpoints in each path.
- The second line contains n integers representing the difficulty levels of Forest Path.
- The third line contains n integers representing the difficulty levels of Cave Path.

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
