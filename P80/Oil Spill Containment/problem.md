## Title
Oil Spill Containment

## Slug
oil-spill-containment

## Difficulty
Medium

## Description
Oil leaked from the Tanker (node 1) and is drifting to the Beach (node n).

The harbor consists of $n$ zones connected by $m$ two-way channels.
The oil is attempting to travel from the Tanker (node 1) to the Beach (node $n$).

To prevent this, you can boom specific channels. Placing a boom in a channel stops the oil.

Your task is to calculate the **minimum number of channels** that must be boomed to completely sever all routes between the Tanker and the Beach.

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
We can boom edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of zones and channels.
- The next $m$ lines describe the channels. Each line contains two integers $a$ and $b$, indicating a channel between zone $a$ and zone $b$.

## Output Format
- Return one integer: the minimum number of channels that need to be boomed.

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
