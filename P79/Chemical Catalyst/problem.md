## Title
Chemical Catalyst

## Slug
chemical-catalyst

## Difficulty
Medium

## Description
Reactants move through a synthesizer. Catalytic tubes are consumed in the reaction.

The synthesizer consists of $n$ vessels and $m$ one-way tubes. Each tube connects a specific source vessel to a destination vessel.

The process happens over several reactions. In each reaction, you must send a reactant batch from vessel 1 (the source) to vessel $n$ (the destination). The catch is that each tube is consumed by the chemical process. This means each tube can be used at most once across all reactions combined.

Your goal is to determine the maximum number of reactions you can successfully complete the journey from vessel 1 to vessel $n$.

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
You can complete 2 reactions.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 reaction.

## Input Format
- The first line contains two integers $n$ and $m$: the number of vessels and the number of tubes.
- The next $m$ lines describe the tubes. Each line contains two integers $a$ and $b$, indicating a directed tube from vessel $a$ to vessel $b$.

## Output Format
- Return one integer: the maximum number of reactions possible.

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
