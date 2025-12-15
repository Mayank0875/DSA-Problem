## Title
Ant Invasion

## Slug
ant-invasion

## Difficulty
Medium

## Description
An invasive ant colony has entered the Kitchen (node 1) and is marching toward the Pantry (node n).

The house consists of $n$ areas connected by $m$ two-way cracks.
The ants is attempting to travel from the Kitchen (node 1) to the Pantry (node $n$).

To prevent this, you can seal specific cracks. Sealing a crack stops the ants.

Your task is to calculate the **minimum number of cracks** that must be sealed to completely sever all routes between the Kitchen and the Pantry.

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
- The first line contains two integers $n$ and $m$: the number of areas and cracks.
- The next $m$ lines describe the cracks. Each line contains two integers $a$ and $b$, indicating a crack between area $a$ and area $b$.

## Output Format
- Return one integer: the minimum number of cracks that need to be sealed.

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
