## Title
Satellite Constellation

## Slug
satellite-constellation

## Difficulty
Hard

## Description
n satellites orbit Earth. Lasers connect some into meshes. The agency wants meshes of 'Signal Size' (digits 4 and 7).

You can calibrate lasers. Merging k meshes requires k - 1 calibrations.

Your task is to determine the minimum number of extra calibrations the agency needs to build to create at least one mesh whose size is a Signal Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect satellite 4 with satellite 3. We can also connect 4 with 1 or 2. This creates a mesh of size 4 (a Signal Size).

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
There is no way to connect the satellites to form a mesh with a size equal to a Signal Size.

## Input Format
- The first line contains two integers n and m: the number of satellites and the number of existing calibrations.
- The next m lines each contain two integers u and v, representing a laser between satellite u and satellite v. Note that u may be equal to v, and there may be multiple calibrations connecting the same pair of satellites.

## Output Format
- Return a single integer: the minimum number of calibrations to build. If no solution exists, print -1.

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
