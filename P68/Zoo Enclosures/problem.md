## Title
Zoo Enclosures

## Slug
zoo-enclosures

## Difficulty
Hard

## Description
n animals are in a zoo. Gates connect some pens into habitats. The vet wants habitats with a 'Healthy Count' of animals (digits 4 and 7).

You can open gates. Merging k habitats requires k - 1 gate operations.

Your task is to determine the minimum number of extra operations the vet needs to build to create at least one habitat whose size is a Healthy Count. If this goal cannot be achieved, return -1.

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
The optimal way is to connect animal 4 with animal 3. We can also connect 4 with 1 or 2. This creates a habitat of size 4 (a Healthy Count).

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
There is no way to connect the animals to form a habitat with a size equal to a Healthy Count.

## Input Format
- The first line contains two integers n and m: the number of animals and the number of existing operations.
- The next m lines each contain two integers u and v, representing a gate between animal u and animal v. Note that u may be equal to v, and there may be multiple operations connecting the same pair of animals.

## Output Format
- Return a single integer: the minimum number of operations to build. If no solution exists, print -1.

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
