## Title
Microchip Data Bus

## Slug
microchip-data-bus

## Difficulty
Medium

## Description
Two parallel data buses on a chip need bridges to route signals around defects.

Two parallel buses, Bus High and Bus Low, each contain n pins arranged in a line.
Bus High has an array `a` representing the clock speed of each pin.
Bus Low has an array `b` representing the clock speed of each pin.

Inside each bus, adjacent pins are already connected by internal traces.

You must establish inter-bus bridges connecting some pins of Bus High to some pins of Bus Low.

The cost to create a bridge between pin i of Bus High and pin j of Bus Low is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single pin is removed (from either Bus High or Bus Low).
If one pin fails and disappears along with all its connections, the remaining pins must still form a single connected network.

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
It's optimal to connect four pairs of pins:
1. pin 1 from Bus High with pin 2 from Bus Low: cost |1-4| = 3.
2. pin 3 from Bus High with pin 2 from Bus Low: cost |1-4| = 3.
3. pin 2 from Bus High with pin 1 from Bus Low: cost |10-20| = 10.
4. pin 2 from Bus High with pin 3 from Bus Low: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first pin of Bus High with the first of Bus Low, and the last pin of Bus High with the last of Bus Low, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of pins in each bus.
- The second line contains n integers representing the clock speeds of Bus High.
- The third line contains n integers representing the clock speeds of Bus Low.

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
