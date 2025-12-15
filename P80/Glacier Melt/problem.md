## Title
Glacier Melt

## Slug
glacier-melt

## Difficulty
Medium

## Description
Meltwater starts at the Glacier Tip (node 1) and flows to the Valley Village (node n).

The mountain face consists of $n$ crevasses connected by $m$ two-way streams.
The water is attempting to travel from the Glacier (node 1) to the Village (node $n$).

To prevent this, you can freeze specific streams. Freezing a stream stops the flow.

Your task is to calculate the **minimum number of streams** that must be frozen to completely sever all routes between the Glacier and the Village.

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
We can freeze edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of crevasses and streams.
- The next $m$ lines describe the streams. Each line contains two integers $a$ and $b$, indicating a stream between crevasse $a$ and crevasse $b$.

## Output Format
- Return one integer: the minimum number of streams that need to be frozen.

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
