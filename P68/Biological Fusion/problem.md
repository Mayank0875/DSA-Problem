## Title
Biological Fusion

## Slug
biological-fusion

## Difficulty
Hard

## Description
Biologists are studying n bacterial colonies in a dish. Protein bridges connect some colonies. A mutation is triggered only when a super-colony has a size equal to a 'Mutagen Number'—composed solely of digits 4 and 7.

You can synthetically create protein bridges to fuse colonies. Fusing k colonies requires k - 1 new bridges.

Your task is to determine the minimum number of extra protein bridges the biologist needs to build to create at least one super-colony whose size is a Mutagen Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect colony 4 with colony 3. We can also connect 4 with 1 or 2. This creates a super-colony of size 4 (a Mutagen Number).

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
There is no way to connect the colonies to form a super-colony with a size equal to a Mutagen Number.

## Input Format
- The first line contains two integers n and m: the number of colonies and the number of existing protein bridges.
- The next m lines each contain two integers u and v, representing a protein bridge between colony u and colony v. Note that u may be equal to v, and there may be multiple protein bridges connecting the same pair of colonies.

## Output Format
- Return a single integer: the minimum number of protein bridges to build. If no solution exists, print -1.

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
