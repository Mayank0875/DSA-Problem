## Title
Crystal Lattice Support

## Slug
crystal-lattice-support

## Difficulty
Medium

## Description
A crystal structure has n atoms. Physicists identify atoms that support the bonds of k other atoms.

The Physicist defines the "Structural Support" of the structure rooted at a specific atom `r` as follows:
Consider every possible set of `k` distinct atoms from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the atoms in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique atoms obtained as LCAs from these sets.
3. The Structural Support of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Lattice Integrity" is defined as the sum of the Structural Support values for all possible roots `r` from 1 to `n`:
Lattice Integrity = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Lattice Integrity of the given molecular structure.

Notes:
1. A molecular structure is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted molecular structure is the deepest node that is an ancestor of all nodes in the set.

## Examples

### 1

#### Input
6 3
1 2
1 3
2 4
2 5
3 6

#### Output
17

#### Explanation
The calculated Lattice Integrity is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Lattice Integrity is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of atoms and the size of the sets to consider.
- The following `n-1` lines describe the molecular structure. Each line contains two integers `u` and `v`, indicating a connection between atoms `u` and `v`.

## Output Format
- Return one integer: the Lattice Integrity.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
