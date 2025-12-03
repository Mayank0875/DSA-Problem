## Title
Solar Panel Strings

## Slug
solar-panel-strings

## Difficulty
Medium

## Description
Two strings of solar panels need cross-wiring to maintain power output if a panel fails.

Two parallel strings, String 1 and String 2, each contain n panels arranged in a line.
String 1 has an array `a` representing the voltage of each panel.
String 2 has an array `b` representing the voltage of each panel.

Inside each string, adjacent panels are already connected by internal series wires.

You must establish inter-string bypass diodes connecting some panels of String 1 to some panels of String 2.

The cost to create a diode between panel i of String 1 and panel j of String 2 is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single panel is removed (from either String 1 or String 2).
If one panel fails and disappears along with all its connections, the remaining panels must still form a single connected network.

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
It's optimal to connect four pairs of panels:
1. panel 1 from String 1 with panel 2 from String 2: cost |1-4| = 3.
2. panel 3 from String 1 with panel 2 from String 2: cost |1-4| = 3.
3. panel 2 from String 1 with panel 1 from String 2: cost |10-20| = 10.
4. panel 2 from String 1 with panel 3 from String 2: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first panel of String 1 with the first of String 2, and the last panel of String 1 with the last of String 2, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of panels in each string.
- The second line contains n integers representing the voltages of String 1.
- The third line contains n integers representing the voltages of String 2.

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
