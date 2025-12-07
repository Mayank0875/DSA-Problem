## Title
Spy Network Cells

## Slug
spy-network-cells

## Difficulty
Medium

## Description
A spy agency organizes agents into independent cells. Each cell is a closed loop of communication. Every agent knows exactly two other agents in their cell.

There are n agents.
Communication loops must have at least 2 agents.
The seized dossier only lists one known contact for each agent.

Your task is to analyze this partial data and determine the minimum and maximum number of separate cells that could possibly exist, consistent with the given records.

## Examples

### 1

#### Input
6
2 1 4 3 6 5

#### Output
1 3

#### Explanation
The records show the connections:
1 <-> 2,
3 <-> 4,
5 <-> 6.
Maximum:
These could be 3 separate cells of 2 agents each.
Minimum:
Since we only know one neighbor per agent, these pairs could actually be segments of a bigger ring. All agents can be arranged into one single ring:
1 - 2 - 3 - 4 - 5 - 6 - 1.

### 2

#### Input
6
2 3 1 5 6 4

#### Output
2 2

#### Explanation
Maximum: 2
Minimum: 2
(Two cycles of length 3 are formed, which are fixed).

## Input Format
- The first line contains an integer n, the number of agents.
- The second line contains n space-separated integers a1, a2, ..., an, where ai is the neighbor remembered by the i-th agent.

## Output Format
- Return two integers: the minimum number of cells and the maximum number of cells.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ ai ≤ 2e5
- ai ≠ i
- The input guarantees that a valid configuration of cells exists.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, connected-components
