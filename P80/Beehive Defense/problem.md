## Title
Beehive Defense

## Slug
beehive-defense

## Difficulty
Medium

## Description
A parasitic wasp entered the Hive Entrance (node 1) and seeks the Larvae Chamber (node n).

The hive consists of $n$ combs connected by $m$ two-way tunnels.
The wasp is attempting to travel from the Entrance (node 1) to the Larvae (node $n$).

To prevent this, you can plug specific tunnels. Plugging a tunnel with wax stops the wasp.

Your task is to calculate the **minimum number of tunnels** that must be plugged to completely sever all routes between the Entrance and the Larvae.

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
We can plug edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of combs and tunnels.
- The next $m$ lines describe the tunnels. Each line contains two integers $a$ and $b$, indicating a tunnel between comb $a$ and comb $b$.

## Output Format
- Return one integer: the minimum number of tunnels that need to be plugged.

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
