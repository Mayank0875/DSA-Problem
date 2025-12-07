## Title
Book Chapter Links

## Slug
book-chapter-links

## Difficulty
Medium

## Description
An interactive book has chapters linking to others. The author wants to bundle linked chapters into episodes. Each chapter belongs to one episode.

The structure is a tree with n chapters and n-1 links.
A episode is formed between two chapters connected by a link.
However, each chapter can be part of at most one episode.

Your task is to calculate the maximum number of episodes that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of episodes is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 episodes.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form episodes (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of chapters.
- The next n-1 lines each contain two integers u and v, representing a link between chapter u and chapter v.

## Output Format
- Return a single integer representing the maximum number of episodes.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
