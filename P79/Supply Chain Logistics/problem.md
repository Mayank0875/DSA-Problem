## Title
Supply Chain Logistics

## Slug
supply-chain-logistics

## Difficulty
Medium

## Description
Goods move from factory to port. Transport contracts are single-use only.

The logistics web consists of $n$ warehouses and $m$ one-way contracts. Each contract connects a specific source warehouse to a destination warehouse.

The process happens over several shipments. In each shipment, you must send a shipment from warehouse 1 (the source) to warehouse $n$ (the destination). The catch is that each contract expires immediately after one shipment is fulfilled. This means each contract can be used at most once across all shipments combined.

Your goal is to determine the maximum number of shipments you can successfully complete the journey from warehouse 1 to warehouse $n$.

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
You can complete 2 shipments.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 shipment.

## Input Format
- The first line contains two integers $n$ and $m$: the number of warehouses and the number of contracts.
- The next $m$ lines describe the contracts. Each line contains two integers $a$ and $b$, indicating a directed contract from warehouse $a$ to warehouse $b$.

## Output Format
- Return one integer: the maximum number of shipments possible.

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
