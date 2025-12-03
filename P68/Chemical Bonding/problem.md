## Title
Chemical Bonding

## Slug
chemical-bonding

## Difficulty
Hard

## Description
n atoms float in a reactor. Bonds connect some into molecules. A catalyst works best on molecules with an 'Atomic Value' of atoms—integers with digits 4 and 7.

A chemist can force new bonds. Merging k molecules requires k - 1 energy bursts.

Your task is to determine the minimum number of extra bonds the chemist needs to build to create at least one molecule whose size is a Atomic Value. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect atom 4 with atom 3. We can also connect 4 with 1 or 2. This creates a molecule of size 4 (a Atomic Value).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the atoms to form a molecule with a size equal to a Atomic Value.

## Input Format
- The first line contains two integers n and m: the number of atoms and the number of existing bonds.
- The next m lines each contain two integers u and v, representing a bond between atom u and atom v. Note that u may be equal to v, and there may be multiple bonds connecting the same pair of atoms.

## Output Format
- Return a single integer: the minimum number of bonds to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
