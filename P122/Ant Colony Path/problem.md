## Title
Ant Colony Path

## Slug
ant-colony-path

## Difficulty
Hard

## Description
An ant leaves pheromones on leaves. It walks to the next leaf or jumps to the second one.

The ant starts at leaf 0 and wishes to reach leaf $n$. On each move, The ant can move forward either **1 leaf** or **2 leaves**.

Your task is to calculate the total number of distinct ways to reach exactly leaf $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach leaf 2:
1. 1 leaf + 1 leaf
2. 2 leaves

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target leaf.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

