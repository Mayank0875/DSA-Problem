## Title
Coral Reef Growth

## Slug
coral-reef-growth

## Difficulty
Hard

## Description
n coral polyps grow on a rock. Calcium bridges connect some into colonies. Marine biologists study colonies of 'Reef Size' (digits 4 and 7).

You can stimulate growth. Merging k colonies requires k - 1 stimuli.

Your task is to determine the minimum number of extra stimuli the biologist needs to build to create at least one colony whose size is a Reef Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect polyp 4 with polyp 3. We can also connect 4 with 1 or 2. This creates a colony of size 4 (a Reef Size).

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
There is no way to connect the polyps to form a colony with a size equal to a Reef Size.

## Input Format
- The first line contains two integers n and m: the number of polyps and the number of existing stimuli.
- The next m lines each contain two integers u and v, representing a bridge between polyp u and polyp v. Note that u may be equal to v, and there may be multiple stimuli connecting the same pair of polyps.

## Output Format
- Return a single integer: the minimum number of stimuli to build. If no solution exists, print -1.

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
