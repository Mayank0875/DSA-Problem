## Title
Desert Caravan Water

## Slug
desert-caravan-water

## Difficulty
Medium

## Description
Caravans travel between oases. Small wells dry up after watering one caravan.

The desert consists of $n$ oases and $m$ one-way routes. Each route connects a specific source oasis to a destination oasis.

The process happens over several caravans. In each caravan, you must send a caravan from oasis 1 (the source) to oasis $n$ (the destination). The catch is that each route drains the water reserves along the way. This means each route can be used at most once across all caravans combined.

Your goal is to determine the maximum number of caravans you can successfully complete the journey from oasis 1 to oasis $n$.

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
You can complete 2 caravans.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 caravan.

## Input Format
- The first line contains two integers $n$ and $m$: the number of oases and the number of routes.
- The next $m$ lines describe the routes. Each line contains two integers $a$ and $b$, indicating a directed route from oasis $a$ to oasis $b$.

## Output Format
- Return one integer: the maximum number of caravans possible.

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
