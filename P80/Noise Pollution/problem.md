## Title
Noise Pollution

## Slug
noise-pollution

## Difficulty
Medium

## Description
Loud music from the Club (node 1) travels to the Library (node n).

The acoustic space consists of $n$ rooms connected by $m$ two-way vents.
The sound is attempting to travel from the Club (node 1) to the Library (node $n$).

To prevent this, you can insulate specific vents. Insulating a vent blocks the sound.

Your task is to calculate the **minimum number of vents** that must be insulated to completely sever all routes between the Club and the Library.

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
We can insulate edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of rooms and vents.
- The next $m$ lines describe the vents. Each line contains two integers $a$ and $b$, indicating a vent between room $a$ and room $b$.

## Output Format
- Return one integer: the minimum number of vents that need to be insulated.

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
