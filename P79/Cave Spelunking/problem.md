## Title
Cave Spelunking

## Slug
cave-spelunking

## Difficulty
Medium

## Description
Explorers squeeze through tight gaps. Loose rocks seal the gap after one person.

The cave consists of $n$ caverns and $m$ one-way squeezes. Each squeeze connects a specific source cavern to a destination cavern.

The process happens over several explorers. In each explorer, you must send a explorer from cavern 1 (the source) to cavern $n$ (the destination). The catch is that each squeeze collapses with loose rock. This means each squeeze can be used at most once across all explorers combined.

Your goal is to determine the maximum number of explorers you can successfully complete the journey from cavern 1 to cavern $n$.

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
You can complete 2 explorers.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 explorer.

## Input Format
- The first line contains two integers $n$ and $m$: the number of caverns and the number of squeezes.
- The next $m$ lines describe the squeezes. Each line contains two integers $a$ and $b$, indicating a directed squeeze from cavern $a$ to cavern $b$.

## Output Format
- Return one integer: the maximum number of explorers possible.

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
