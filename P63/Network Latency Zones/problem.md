## Title
Network Latency Zones

## Slug
network-latency-zones

## Difficulty
Easy

## Description
A network path consists of $n$ hops. Each hop is classified into 5 latency zones (Zone 1 to 5). In an optimized route, the latency zone of subsequent hops never decreases (traffic moves away from the core). Count the valid route profiles.

## Examples

### 1

#### Input
1

#### Output
5

#### Explanation
There are 5 valid sequences of length 1.

### 2

#### Input
2

#### Output
15

#### Explanation
There are 15 valid sorted sequences of length 2 (e.g., aa, ae, ai, ao, au, ee, etc.).

## Input Format
- The input consists of a single integer n, representing the required length/quantity.

## Output Format
- Return a single integer representing the total number of valid sorted sequences.

## Constraints
- 1 ≤ n ≤ 50

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math
