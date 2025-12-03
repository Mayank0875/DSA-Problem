## Title
Circuit Board Design

## Slug
circuit-board-design

## Difficulty
Hard

## Description
n pins are on a board. Traces connect some into nets. The design requires nets with a 'Conductive Count' of pins (digits 4 and 7).

An engineer can solder new traces. Merging k nets requires k - 1 traces.

Your task is to determine the minimum number of extra traces the engineer needs to build to create at least one net whose size is a Conductive Count. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect pin 4 with pin 3. We can also connect 4 with 1 or 2. This creates a net of size 4 (a Conductive Count).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the pins to form a net with a size equal to a Conductive Count.

## Input Format
- The first line contains two integers n and m: the number of pins and the number of existing traces.
- The next m lines each contain two integers u and v, representing a trace between pin u and pin v. Note that u may be equal to v, and there may be multiple traces connecting the same pair of pins.

## Output Format
- Return a single integer: the minimum number of traces to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
