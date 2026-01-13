## Title
Rocket Thrust

## Slug
rocket-thrust

## Difficulty
Easy

## Description
Engineers test thrusters. They rank them by force generated.

The test stand records the thrust (kN) of $N$ thrusters in an array. To select the engine, the engineer needs to assign a rank to every thruster based on its thrust (kN).

The ranking rules are simple: the thruster with the **smallest** thrust (kN) gets **Rank 1**. The next distinct thrust (kN) gets **Rank 2**, and so on.

If two or more thrusters have the exact same thrust (kN), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each thruster's thrust (kN) with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All thrusters share the same thrust (kN), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of thrusters.
- The second line contains `n` space-separated integers representing the thrust (kN)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding thruster.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
