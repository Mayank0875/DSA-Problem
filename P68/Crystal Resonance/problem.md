## Title
Crystal Resonance

## Slug
crystal-resonance

## Difficulty
Hard

## Description
In a cave, n magic crystals glow. Ley lines connect some crystals into resonance groups. A group achieves maximum power if its size is a 'Mana Number'—an integer with only digits 4 and 7.

A mage can draw new ley lines to merge groups. Merging k groups requires casting k - 1 ley line spells.

Your task is to determine the minimum number of extra ley lines the mage needs to build to create at least one resonance group whose size is a Mana Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect crystal 4 with crystal 3. We can also connect 4 with 1 or 2. This creates a resonance group of size 4 (a Mana Number).

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
There is no way to connect the crystals to form a resonance group with a size equal to a Mana Number.

## Input Format
- The first line contains two integers n and m: the number of crystals and the number of existing ley lines.
- The next m lines each contain two integers u and v, representing a ley line between crystal u and crystal v. Note that u may be equal to v, and there may be multiple ley lines connecting the same pair of crystals.

## Output Format
- Return a single integer: the minimum number of ley lines to build. If no solution exists, print -1.

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
