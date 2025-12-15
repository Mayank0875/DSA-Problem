## Title

Interstellar Cargo Relay

## Slug

interstellar-cargo-relay

## Difficulty

Medium

## Description

In the year 3055, the Interstellar Trade Federation manages a network of $n$ space stations connected by $m$ one-way wormholes. Each wormhole connects a source station to a destination station and requires a specific amount of fuel units to traverse.

You are a logistics officer tasked with routing a critical shipment from Earth (station 1) to the Federation Headquarters (station $n$). Due to strict quantization protocols in the ship's navigation computer, the journey must consist of exactly $k$ wormhole jumps.

Your goal is to calculate the minimum total fuel required to travel from station 1 to station $n$ using exactly $k$ jumps. If it is impossible to reach the destination with exactly $k$ jumps, you must report that the route is invalid.

## Examples

### 1

#### Input

3 4 8
1 2 5
2 3 4
3 1 1
3 2 2

#### Output

27

#### Explanation

We need a path from node 1 to node 3 using exactly 8 edges.
First try this path:
1 → 2 → 3 → 1 → 2 → 3 → 1 → 2 → 3
Edge costs: 5 + 4 + 1 + 5 + 4 + 1 + 5 + 4 = 29
Now check if there's a better one.
Try this path:
1 → 2 → 3 → 2 → 3 → 2 → 3 → 2 → 3
Edge costs: 5 + 4 + 2 + 4 + 2 + 4 + 2 + 4 = 27
So the minimum total cost for a path of length 8 from node 1 to node 3 is 27.
    
### 2

#### Input

2 1 100
1 2 10

#### Output

-1

#### Explanation

There is only one edge 1 → 2. It is impossible to make 100 jumps because once you reach node 2, there are no outgoing edges to continue the journey.
  

## Input Format  

- The first line contains three integers $n$, $m$, and $k$: the number of stations, wormholes, and the required number of jumps.
- The next $m$ lines describe the wormholes. Each line contains three integers $a$, $b$, and $c$: there is a wormhole from station $a$ to station $b$ with a fuel cost of $c$.

## Output Format  

- Return minimum total fuel cost. If no such path exists, print -1.
  

## Constraints  

- 1 ≤ n ≤ 100
- 1 ≤ m ≤ (n * (n - 1))
- 1 ≤ k ≤ 1e9
- 1 ≤ a, b ≤ n
- 1 ≤ c ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, dynamic-programming