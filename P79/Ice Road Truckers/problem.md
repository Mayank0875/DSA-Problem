## Title
Ice Road Truckers

## Slug
ice-road-truckers

## Difficulty
Medium

## Description
Trucks cross frozen lakes. The ice cracks and becomes unsafe after one truck.

The tundra consists of $n$ towns and $m$ one-way ice roads. Each ice road connects a specific source town to a destination town.

The process happens over several trucks. In each truck, you must send a truck from town 1 (the source) to town $n$ (the destination). The catch is that each ice road cracks and becomes too dangerous for a second pass. This means each ice road can be used at most once across all trucks combined.

Your goal is to determine the maximum number of trucks you can successfully complete the journey from town 1 to town $n$.

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
You can complete 2 trucks.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 truck.

## Input Format
- The first line contains two integers $n$ and $m$: the number of towns and the number of ice roads.
- The next $m$ lines describe the ice roads. Each line contains two integers $a$ and $b$, indicating a directed ice road from town $a$ to town $b$.

## Output Format
- Return one integer: the maximum number of trucks possible.

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
