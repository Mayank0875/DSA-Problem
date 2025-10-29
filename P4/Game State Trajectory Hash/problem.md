## Title

Game State Trajectory Hash

## Slug

game-state-trajectory-hash

## Difficulty

Easy

## Description

In a simulation game, the state is represented by a sequence of numerical parameters A₁, A₂, ..., Aₙ recorded over time. A game analyst wants to understand the dynamics over short intervals. They use a sliding window of size K to capture snapshots of the game state. For each snapshot (window), they compute a hash value by XORing the parameters inside it. To get a single value representing the overall trajectory's characteristics, they XOR all these snapshot hashes together. Compute this final trajectory hash.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

State snapshots (windows) of size 3:
    •   [1, 2, 3] → Snapshot Hash (XOR) = 0
    •   [2, 3, 4] → Snapshot Hash (XOR) = 5
    •   [3, 4, 5] → Snapshot Hash (XOR) = 2

Final Trajectory Hash = 0 ^ 5 ^ 2 = 7

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

7

#### Explanation

Snapshots:
    •   [5, 1] → XOR = 4
    •   [1, 3] → XOR = 2
    •   [3, 2] → XOR = 1

Final Trajectory Hash = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of parameters) and K (snapshot size).
- The second line contains N space-separated integers — the parameter values.

## Output Format

- Return a single integer — the final trajectory hash.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, game development, bit manipulation