## Title
Concert Sound System

## Slug
concert-sound-system

## Difficulty
Hard

## Description
Audio signals travel from the microphone to the main speakers. Cables and amplifiers have signal power limits.

The network consists of n amps, numbered 1 to n.
1. Amp 1 is the Microphone.
2. Amp n is the Speaker.

There are m one-way cables connecting these amps. Each cable has a specific capacity, measured in signal power units, which limits the rate at which sound can flow through it.

Multiple cables can exist between the same two amps, and their capacities stack. Your goal is to determine the maximum total audio output that can be achieved from the Microphone to the Speaker using the available network.

## Examples

### 1

#### Input
4 5
1 2 3
2 4 2
1 3 4
3 4 5
4 1 3

#### Output
6

#### Explanation
There are two main paths to transmit sound from node 1 to node 4:
1 -> 2 -> 4 (capacity limited by link 2 -> 4 with capacity 2).
1 -> 3 -> 4 (capacity limited by link 1 -> 3 with capacity 4).
Total max flow is 2 + 4 = 6. The link 4 -> 1 is ignored because it flows backward from the destination.

### 2

#### Input
3 2
1 2 5
2 3 5

#### Output
5

#### Explanation
A single path 1 -> 2 -> 3 exists with a bottleneck capacity of 5.

## Input Format
- The first line contains two integers n and m: the number of amps and the number of cables.
- The next m lines describe the cables. Each line contains three integers u, v, and c, indicating a one-way cable from Amp u to Amp v with capacity c.

## Output Format
- Return one integer: the maximum audio output from Amp 1 to Amp n.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ u, v ≤ n
- 1 ≤ c ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
