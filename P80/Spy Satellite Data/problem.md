## Title
Spy Satellite Data

## Slug
spy-satellite-data

## Difficulty
Medium

## Description
A rogue satellite (node 1) attempts to beam data to a Ground Station (node n).

The satellite mesh consists of $n$ relays connected by $m$ two-way beams.
The data is attempting to travel from the Satellite (node 1) to the Ground (node $n$).

To prevent this, you can jam specific beams. Jamming a beam stops transmission.

Your task is to calculate the **minimum number of beams** that must be jammed to completely sever all routes between the Satellite and the Ground.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can jam edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of relays and beams.
- The next $m$ lines describe the beams. Each line contains two integers $a$ and $b$, indicating a beam between relay $a$ and relay $b$.

## Output Format
- Return one integer: the minimum number of beams that need to be jammed.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
