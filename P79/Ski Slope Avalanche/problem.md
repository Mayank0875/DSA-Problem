## Title
Ski Slope Avalanche

## Slug
ski-slope-avalanche

## Difficulty
Medium

## Description
Skiers go off-piste. Unstable snow slides after being disturbed once.

The resort consists of $n$ lodges and $m$ one-way slopes. Each slope connects a specific source lodge to a destination lodge.

The process happens over several skiers. In each skier, you must send a skier from lodge 1 (the source) to lodge $n$ (the destination). The catch is that each slope triggers a small slide, ruining the powder. This means each slope can be used at most once across all skiers combined.

Your goal is to determine the maximum number of skiers you can successfully complete the journey from lodge 1 to lodge $n$.

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
You can complete 2 skiers.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 skier.

## Input Format
- The first line contains two integers $n$ and $m$: the number of lodges and the number of slopes.
- The next $m$ lines describe the slopes. Each line contains two integers $a$ and $b$, indicating a directed slope from lodge $a$ to lodge $b$.

## Output Format
- Return one integer: the maximum number of skiers possible.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
