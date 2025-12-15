## Title

One-Way Teleporter Network

## Slug

one-way-teleporter-network

## Difficulty

Medium

## Description

A futuristic game is played in a space station consisting of $n$ rooms and $m$ one-way teleporters. Each teleporter connects a specific source room to a destination room.

The game is played over several days. On each day, you must travel from room 1 (the starting point) to room $n$ (the extraction point). The catch is that each teleporter consumes a rare energy crystal upon use and collapses permanently. This means each teleporter can be used at most once across all days combined.

Your goal is to determine the maximum number of days you can successfully complete the journey from room 1 to room $n$.

## Examples

### 1

#### Input

6 7
1 2
1 3
2 6
3 4
3 5
4 6
5 6

#### Output

2

#### Explanation

You can play for 2 days.
    
### 2

#### Input

2 1
1 2

#### Output

1

#### Explanation

You can play for 1 days.
  

## Input Format  

- The first line contains two integers $n$ and $m$: the number of rooms and the number of teleporters.
- The next $m$ lines describe the teleporters. Each line contains two integers $a$ and $b$, indicating a directed teleporter from room $a$ to room $b$.

## Output Format  

- Return one integer: the maximum number of days you can play the game.
  

## Constraints  

- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, breadth-first-search, hackwithinfy

## Companies
infosys