## Title
Logic Gate Oscillation

## Slug
logic-gate-oscillation

## Difficulty
Medium

## Description
Digital circuits use feedback. A ring oscillator is a loop of gates.

A "oscillator ring" occurs when a signal moves from a gate, through a sequence of wires, and returns to the starting gate without traversing the same wire twice in immediate succession. The "length" of such a oscillator ring is the number of wires it contains.

Find the number of gates in the smallest oscillator.

Given the layout of the chip, determine the length of the shortest oscillator ring.

## Examples

### 1

#### Input
5 6
1 2
1 3
2 4
2 5
3 4
4 5

#### Output
3

#### Explanation
There are several oscillator rings in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest oscillator ring has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no oscillator rings in this network.

## Input Format
- The first line contains two integers n and m: the number of gates and the number of wires.
- The gates are numbered 1, 2, ..., n.
- The next m lines describe the wires. Each line contains two integers u and v, indicating a connection between gate u and gate v.
- The graph is undirected. There is at most one wire between any two gates.

## Output Format
- Return one integer: the length of the shortest oscillator ring. If there are no oscillator rings, print `-1`.

## Constraints
- 1 ≤ n ≤ 2500
- 1 ≤ m ≤ 5000
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
