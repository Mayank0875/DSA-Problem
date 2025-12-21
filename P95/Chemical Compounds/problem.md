## Title
Chemical Compounds

## Slug
chemical-compounds

## Difficulty
Hard

## Description
Atoms are bonded into molecules. The classification of a molecule is based on its most abundant atom ID.

The Chemist has a collection of $n$ atoms, where each atom is represented by an integer ID.

To synthesize materials, The Chemist must partition these atoms into several non-empty molecules. Every atom from the original collection must belong to exactly one molecule. From each molecule, a "classification" is extracted. The classification is defined as the **mode** (most frequent element) of the atoms in that molecule. If a molecule has multiple atoms tied for the most frequent appearance, any one of them can be chosen as the classification.

The Chemist collects all the extracted classifications to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> classification is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> classifications 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> classifications 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> classifications 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of atoms.
- The second line contains $n$ space-separated integers representing the atom IDs.

## Output Format
- Return a single integer representing the number of different multisets of classifications possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
