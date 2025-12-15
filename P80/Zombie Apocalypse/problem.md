## Title
Zombie Apocalypse

## Slug
zombie-apocalypse

## Difficulty
Medium

## Description
Zombies have breached the West Wall (node 1) and are swarming toward the Survivors' Camp (node n).

The city consists of $n$ blocks connected by $m$ two-way streets.
The horde is attempting to travel from the Wall (node 1) to the Camp (node $n$).

To prevent this, you can barricade specific streets. Barricading a street stops the zombies.

Your task is to calculate the **minimum number of streets** that must be barricaded to completely sever all routes between the Wall and the Camp.

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
We can barricade edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of blocks and streets.
- The next $m$ lines describe the streets. Each line contains two integers $a$ and $b$, indicating a street between block $a$ and block $b$.

## Output Format
- Return one integer: the minimum number of streets that need to be barricaded.

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
