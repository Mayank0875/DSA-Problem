## Title
Art Gallery Exhibition

## Slug
art-gallery-exhibition

## Difficulty
Medium

## Description
A curator places `n` paintings on `m` walls.

However, not every painting is compatible with every wall due to lighting requirements.
You are given a list of `k` compatible pairs, where a specific painting can work with a specific wall.

Your task is to determine the maximum number of displays that can be formed simultaneously. Each painting and each wall can be assigned to at most one display.

## Examples

### 1

#### Input
3 2 4
1 1
1 2
2 1
3 1

#### Output
2

#### Explanation
There are 3 paintings and 2 walls.
Possible valid matching could be:
- painting 1 with wall 2
- painting 2 with wall 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only painting 1 and wall 1 are compatible. The maximum number of operational displays is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of paintings, walls, and compatible pairs.
- The paintings are numbered `1` to `n` and the walls are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that painting `a` and wall `b` are compatible.

## Output Format
- Return one integer: the maximum number of pairs that can be formed.

## Constraints
- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
