## Title
Quantum Particle Collision

## Slug
quantum-particle-collision

## Difficulty
Easy

## Description
In a high-energy physics laboratory, scientists are smashing particles together to discover new elements. According to the facility's simplified energy model, the kinetic energy release of a particle collision is proportional to the square of its mass. To stabilize a microscopic black hole, the scientists need to collide exactly three particles simultaneously such that their total energy release equals a specific critical threshold. You are given a list of available particles and their masses. You need to check if any trio exists that meets the energy requirement.

Your task is to determine whether it is possible to choose three distinct particles (at indices i < j < k) such that:

    mass_i^2 + mass_j^2 + mass_k^2 = target_energy

If it is possible, print YES; otherwise, print NO.

## Examples

### 1
#### Input
5
1 2 2 3 4
9

#### Output
YES

#### Explanation
1^2 + 2^2 + 2^2 = 1 + 4 + 4 = 9.

### 2
#### Input
4
3 3 3 3
20

#### Output
NO

#### Explanation
Every square is 9; any sum of three squares is 27 which is not 20.

## Input Format
- First line: integer n — the number of particles.
- Second line: n space-separated integers a1 a2 ... an — the mass values (can be negative, zero, or positive).
- Third line: integer target — the target sum.

## Output Format
- Return true (YES) if there exist indices i < j < k with a[i]^2 + a[j]^2 + a[k]^2 = target, otherwise return false (NO).

## Constraints
- 3 ≤ n ≤ 2000
- -10^6 ≤ ai ≤ 10^6
- 0 ≤ target ≤ 3×10^12

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
two-pointers, sorting, array, maths
