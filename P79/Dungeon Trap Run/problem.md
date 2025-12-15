## Title
Dungeon Trap Run

## Slug
dungeon-trap-run

## Difficulty
Medium

## Description
Adventurers run a gauntlet. Traps trigger and block the hallway after one person passes.

The dungeon consists of $n$ rooms and $m$ one-way hallways. Each hallway connects a specific source room to a destination room.

The process happens over several heroes. In each hero, you must send a hero from room 1 (the source) to room $n$ (the destination). The catch is that each hallway triggers a ceiling collapse after use. This means each hallway can be used at most once across all heroes combined.

Your goal is to determine the maximum number of heroes you can successfully complete the journey from room 1 to room $n$.

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
You can complete 2 heroes.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 hero.

## Input Format
- The first line contains two integers $n$ and $m$: the number of rooms and the number of hallways.
- The next $m$ lines describe the hallways. Each line contains two integers $a$ and $b$, indicating a directed hallway from room $a$ to room $b$.

## Output Format
- Return one integer: the maximum number of heroes possible.

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
