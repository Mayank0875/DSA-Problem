## Title
Audio Cable Patching

## Slug
audio-cable-patching

## Difficulty
Medium

## Description
Two audio channels need patch cables to reroute sound if a mixer channel blows.

Two parallel channels, Left Channel and Right Channel, each contain n jacks arranged in a line.
Left Channel has an array `a` representing the impedance of each jack.
Right Channel has an array `b` representing the impedance of each jack.

Inside each channel, adjacent jacks are already connected by internal wires.

You must establish inter-channel patch cables connecting some jacks of Left Channel to some jacks of Right Channel.

The cost to create a cable between jack i of Left Channel and jack j of Right Channel is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single jack is removed (from either Left Channel or Right Channel).
If one jack fails and disappears along with all its connections, the remaining jacks must still form a single connected network.

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
It's optimal to connect four pairs of jacks:
1. jack 1 from Left Channel with jack 2 from Right Channel: cost |1-4| = 3.
2. jack 3 from Left Channel with jack 2 from Right Channel: cost |1-4| = 3.
3. jack 2 from Left Channel with jack 1 from Right Channel: cost |10-20| = 10.
4. jack 2 from Left Channel with jack 3 from Right Channel: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first jack of Left Channel with the first of Right Channel, and the last jack of Left Channel with the last of Right Channel, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of jacks in each channel.
- The second line contains n integers representing the impedances of Left Channel.
- The third line contains n integers representing the impedances of Right Channel.

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
