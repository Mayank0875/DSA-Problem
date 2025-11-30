## Title

Ash and the Tree Cycles

## Slug

ash-and-the-tree-cycles

## Difficulty

Medium

## Description

Ash is designing a magical communication network in a forest. The forest consists of $n$ clearings connected by $n-1$ magical trails, forming a tree structure.

Ash wants to enhance the network's resilience by adding new magical links. A new link can be created between any two clearings that are not already directly connected. When a new link is added between two clearings $u$ and $v$, it creates a cycle consisting of the new link and the unique existing path between $u$ and $v$ in the tree.

However, to prevent magical interference, Ash must ensure that **no two cycles share an edge**. In other words, every edge in the final graph (both original trails and new links) must belong to at most one simple cycle.

Your task is to help Ash calculate the **maximum number of new links** he can add to the forest while satisfying this condition.

## Examples

### 1

#### Input

5
1 2
1 3
1 4
1 5

#### Output

2

#### Explanation

Add Edges bewteen (2, 3) and (4, 5).
    
### 2

#### Input

3
1 2
1 3

#### Output

1

#### Explanation

Add edge bewteen (2, 3).
  

## Input Format  

- The first line contains an integer $n$, the number of clearings.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a trail between clearings $u$ and $v$.

## Output Format  

- Return single integer representing the maximum number of new links Ash can add.
  

## Constraints  

- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ 2e5
- The input guarantees that the graph is a tree.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

tree

## Companies
infosys