## Title
Museum Exhibit

## Slug
museum-exhibit

## Difficulty
Hard

## Description
n artifacts are on display. Walkways connect some into galleries. The curator wants galleries of 'Aesthetic Size' (digits 4 and 7).

New walkways can be built. Merging k galleries costs k - 1 walkways.

Your task is to determine the minimum number of extra walkways the curator needs to build to create at least one gallery whose size is a Aesthetic Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect artifact 4 with artifact 3. We can also connect 4 with 1 or 2. This creates a gallery of size 4 (a Aesthetic Size).

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
There is no way to connect the artifacts to form a gallery with a size equal to a Aesthetic Size.

## Input Format
- The first line contains two integers n and m: the number of artifacts and the number of existing walkways.
- The next m lines each contain two integers u and v, representing a walkway between artifact u and artifact v. Note that u may be equal to v, and there may be multiple walkways connecting the same pair of artifacts.

## Output Format
- Return a single integer: the minimum number of walkways to build. If no solution exists, print -1.

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
