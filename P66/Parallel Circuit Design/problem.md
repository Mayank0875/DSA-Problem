## Title
Parallel Circuit Design

## Slug
parallel-circuit-design

## Difficulty
Medium

## Description
An electrical engineer is designing a fault-tolerant circuit board with two parallel traces.

Two parallel traces, Trace VCC and Trace GND, each contain n pads arranged in a line.
Trace VCC has an array `a` representing the voltage potential of each pad.
Trace GND has an array `b` representing the voltage potential of each pad.

Inside each trace, adjacent pads are already connected by internal copper tracks.

You must establish inter-trace jumpers connecting some pads of Trace VCC to some pads of Trace GND.

The cost to create a jumper between pad i of Trace VCC and pad j of Trace GND is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single pad is removed (from either Trace VCC or Trace GND).
If one pad fails and disappears along with all its connections, the remaining pads must still form a single connected network.

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
It's optimal to connect four pairs of pads:
1. pad 1 from Trace VCC with pad 2 from Trace GND: cost |1-4| = 3.
2. pad 3 from Trace VCC with pad 2 from Trace GND: cost |1-4| = 3.
3. pad 2 from Trace VCC with pad 1 from Trace GND: cost |10-20| = 10.
4. pad 2 from Trace VCC with pad 3 from Trace GND: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first pad of Trace VCC with the first of Trace GND, and the last pad of Trace VCC with the last of Trace GND, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of pads in each trace.
- The second line contains n integers representing the voltage potentials of Trace VCC.
- The third line contains n integers representing the voltage potentials of Trace GND.

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
