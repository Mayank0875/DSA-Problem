## Title
Recipe Substitutions

## Slug
recipe-substitutions

## Difficulty
Medium

## Description
Ingredients can be substituted. A Flavor Group is a set of ingredients that can be swapped cyclically.

Two ingredients a and b belong to the same Flavor Group if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of substitutions.
In other words, two ingredients are in the same Flavor Group if they are mutually reachable.

Your task is to: Determine how many Flavor Groups exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The ingredients form two distinct groups where round-trip traversal is possible within each group.
Ingredients {1, 2, 3} form one Flavor Group.
Path: 1 -> 2 -> 3 -> 1.
Ingredients {4, 5} form another Flavor Group.
Path: 4 -> 5 -> 4.
Total Flavor Groups: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 ingredients and 1 one-way substitution.
Substitution: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Flavor Groups.

## Input Format
- The first line contains two integers n and m: the number of ingredients and substitutions.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way substitution from ingredient a to ingredient b.

## Output Format
- Return one integer: the total number of Flavor Groups.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
