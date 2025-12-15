## Title
Space Station Escape

## Slug
space-station-escape

## Difficulty
Medium

## Description
A station is collapsing. Escape pods must launch from the Command Deck to the Hangar. Corridors are unstable.

The station consists of $n$ modules and $m$ one-way corridors. Each corridor connects a specific source module to a destination module.

The process happens over several evacuation waves. In each wave, you must send a survivor group from module 1 (the source) to module $n$ (the destination). The catch is that each corridor collapses immediately after someone passes through it. This means each corridor can be used at most once across all evacuation waves combined.

Your goal is to determine the maximum number of evacuation waves you can successfully complete the journey from module 1 to module $n$.

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
You can complete 2 evacuation waves.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 wave.

## Input Format
- The first line contains two integers $n$ and $m$: the number of modules and the number of corridors.
- The next $m$ lines describe the corridors. Each line contains two integers $a$ and $b$, indicating a directed corridor from module $a$ to module $b$.

## Output Format
- Return one integer: the maximum number of evacuation waves possible.

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
