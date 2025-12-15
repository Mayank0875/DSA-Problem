## Title
Space Station Airlock

## Slug
space-station-airlock

## Difficulty
Medium

## Description
Aliens have boarded at Airlock 1 and are heading for the Bridge (node n).

The station consists of $n$ modules connected by $m$ two-way hallways.
The aliens is attempting to travel from Airlock 1 (node 1) to the Bridge (node $n$).

To prevent this, you can seal specific hallways. Sealing a hallway isolates the sectors.

Your task is to calculate the **minimum number of hallways** that must be sealed to completely sever all routes between Airlock 1 and the Bridge.

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
We can seal edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of modules and hallways.
- The next $m$ lines describe the hallways. Each line contains two integers $a$ and $b$, indicating a hallway between module $a$ and module $b$.

## Output Format
- Return one integer: the minimum number of hallways that need to be sealed.

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
