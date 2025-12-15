## Title

Mystic Island Guilds

## Slug

mystic-island-guilds

## Difficulty

Medium

## Description

In a mystical archipelago, there are n floating islands connected by m ancient, one-way teleporters.
Each teleporter allows travel from one island to another in a directed manner.

Two islands a and b belong to the same Guild if and only if: It is possible to travel from a to b, and It is also possible to travel from b to a using the network of teleporters.
In other words, two islands are in the same Guild if they are mutually reachable.
A lone cartographer wants to map out the political structure of the archipelago.
Your task is to: Determine how many Guilds exist in total.
Two islands should have the same Guild ID if they belong to the same Guild.

## Examples

### 1

#### Input

5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output

2

#### Explanation

The islands form two distinct groups where round-trip travel is possible within each group.
Islands {1, 2, 3} form one Guild.
Example path: 1 → 2 → 3 → 1 (you can go around and return).
Islands {4, 5} form another Guild.
Example path: 4 → 5 → 4 (round trip possible).

There are 2 Guilds in total.
Islands 1, 2, and 3 are assigned Guild ID 1.
Islands 4 and 5 are assigned Guild ID 2.
    
### 2

#### Input

2 1
1 2

#### Output

2

#### Explanation

There are 2 islands and 1 one-way teleporter.

Teleporter: 1 → 2
(You can travel from island 1 to island 2, but there is no path from 2 back to 1.)
  

## Input Format  

- The first line contains two integers n and m: the number of islands and teleporters.
- The following m lines describe the teleporters. Each line has two integers a and b, indicating a one-way teleporter from island a to island b.

## Output Format  

- Return one integer: the total number of Guilds.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, depth-first-search, hackwithinfy

## Companies
infosys