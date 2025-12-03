## Title
Genetic Ancestry

## Slug
genetic-ancestry

## Difficulty
Hard

## Description
n individuals are in a database. Family trees link some. Researchers look for lineages of 'Marker Size' (digits 4 and 7).

You can find missing links. Merging k lineages requires k - 1 new links.

Your task is to determine the minimum number of extra links the researcher needs to build to create at least one lineage whose size is a Marker Size. If this goal cannot be achieved, return -1.

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
The optimal way is to connect individual 4 with individual 3. We can also connect 4 with 1 or 2. This creates a lineage of size 4 (a Marker Size).

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
There is no way to connect the individuals to form a lineage with a size equal to a Marker Size.

## Input Format
- The first line contains two integers n and m: the number of individuals and the number of existing links.
- The next m lines each contain two integers u and v, representing a link between individual u and individual v. Note that u may be equal to v, and there may be multiple links connecting the same pair of individuals.

## Output Format
- Return a single integer: the minimum number of links to build. If no solution exists, print -1.

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
