## Title
Quantum Entanglement

## Slug
quantum-entanglement

## Difficulty
Medium

## Description
Qubits teleport state. Entanglement is broken (consumed) upon measurement/use.

The quantum computer consists of $n$ qubits and $m$ one-way channels. Each channel connects a specific source qubit to a destination qubit.

The process happens over several states. In each state, you must send a state from qubit 1 (the source) to qubit $n$ (the destination). The catch is that each channel collapses the quantum entanglement. This means each channel can be used at most once across all states combined.

Your goal is to determine the maximum number of states you can successfully complete the journey from qubit 1 to qubit $n$.

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
You can complete 2 states.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 state.

## Input Format
- The first line contains two integers $n$ and $m$: the number of qubits and the number of channels.
- The next $m$ lines describe the channels. Each line contains two integers $a$ and $b$, indicating a directed channel from qubit $a$ to qubit $b$.

## Output Format
- Return one integer: the maximum number of states possible.

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
