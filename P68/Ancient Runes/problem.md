## Title
Ancient Runes

## Slug
ancient-runes

## Difficulty
Hard

## Description
n runes are carved on a wall. Magic lines connect some into spells. A wizard wants spells of 'Power Number' (digits 4 and 7).

You can draw lines. Merging k spells requires k - 1 lines.

Your task is to determine the minimum number of extra lines the wizard needs to build to create at least one spell whose size is a Power Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect rune 4 with rune 3. We can also connect 4 with 1 or 2. This creates a spell of size 4 (a Power Number).

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
There is no way to connect the runes to form a spell with a size equal to a Power Number.

## Input Format
- The first line contains two integers n and m: the number of runes and the number of existing lines.
- The next m lines each contain two integers u and v, representing a line between rune u and rune v. Note that u may be equal to v, and there may be multiple lines connecting the same pair of runes.

## Output Format
- Return a single integer: the minimum number of lines to build. If no solution exists, print -1.

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
