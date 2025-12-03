## Title
Constellation Mapping

## Slug
constellation-mapping

## Difficulty
Hard

## Description
n stars are in the sky. Imaginary lines connect some into constellations. Astrologers seek constellations of 'Zodiac Size' (digits 4 and 7).

You can draw new lines. Merging k constellations requires k - 1 lines.

Your task is to determine the minimum number of extra lines the astrologer needs to build to create at least one constellation whose size is a Zodiac Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect star 4 with star 3. We can also connect 4 with 1 or 2. This creates a constellation of size 4 (a Zodiac Size).

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
There is no way to connect the stars to form a constellation with a size equal to a Zodiac Size.

## Input Format
- The first line contains two integers n and m: the number of stars and the number of existing lines.
- The next m lines each contain two integers u and v, representing a line between star u and star v. Note that u may be equal to v, and there may be multiple lines connecting the same pair of stars.

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
