## Title
Magical Mana Flow

## Slug
magical-mana-flow

## Difficulty
Medium

## Description
Mages channel mana. Leylines burn out from magical stress after one pulse.

The grid consists of $n$ runestones and $m$ one-way leylines. Each leyline connects a specific source runestone to a destination runestone.

The process happens over several pulses. In each pulse, you must send a mana pulse from runestone 1 (the source) to runestone $n$ (the destination). The catch is that each leyline burns out and becomes inert after channeling energy. This means each leyline can be used at most once across all pulses combined.

Your goal is to determine the maximum number of pulses you can successfully complete the journey from runestone 1 to runestone $n$.

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
You can complete 2 pulses.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 pulse.

## Input Format
- The first line contains two integers $n$ and $m$: the number of runestones and the number of leylines.
- The next $m$ lines describe the leylines. Each line contains two integers $a$ and $b$, indicating a directed leyline from runestone $a$ to runestone $b$.

## Output Format
- Return one integer: the maximum number of pulses possible.

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
