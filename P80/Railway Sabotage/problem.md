## Title
Railway Sabotage

## Slug
railway-sabotage

## Difficulty
Medium

## Description
A runaway train left the Depot (node 1) and is heading for the Capital (node n).

The rail network consists of $n$ stations connected by $m$ two-way tracks.
The train is attempting to travel from the Depot (node 1) to the Capital (node $n$).

To prevent this, you can switch specific tracks. Derailing at a track section stops the train.

Your task is to calculate the **minimum number of tracks** that must be derailed to completely sever all routes between the Depot and the Capital.

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
We can switch edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of stations and tracks.
- The next $m$ lines describe the tracks. Each line contains two integers $a$ and $b$, indicating a track between station $a$ and station $b$.

## Output Format
- Return one integer: the minimum number of tracks that need to be derailed.

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
