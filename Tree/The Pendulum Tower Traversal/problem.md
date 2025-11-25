## Title

The Pendulum Tower Traversal

## Slug

the-pendulum-tower-traversal

## Difficulty

Medium

## Description

In the mystical Pendulum Tower, magical energy flows in alternating directions. The tower is constructed as a binary tree hierarchy. To harmoniously collect the energy orbs located in each chamber, a wizard must traverse the tower levels in a specific zigzag pattern.

Starting from the pinnacle (root), the wizard collects orbs from left to right on the first level. However, due to the tower's enchantment, the direction reverses for the next level, requiring a traversal from right to left. This pattern continues, alternating the direction for every subsequent level deeper into the tower. Your task is to simulate this journey and return the sequence of energy values collected by the wizard.

## Examples

### 1

#### Input

7
1 2 3 4 5 6 7

#### Output

1 3 2 4 5 6 7

#### Explanation

Level 1 (L->R): 1
Level 2 (R->L): 3, 2
Level 3 (L->R): 4, 5, 6, 7
Final path: [1, 3, 2, 4, 5, 6, 7]
    
### 2

#### Input

9
7 9 7 8 8 6 null 10 9

#### Output

7 7 9 8 8 6 9 10

#### Explanation

Level 1 (L->R): 7
Level 2 (R->L): 7, 9
Level 3 (L->R): 8, 8, 6
Level 4 (R->L): 9, 10
  

## Input Format  

- The first line contains an integer $n$, representing the number of nodes in the level-order representation of the tree.
- The second line contains $n$ space-separated strings representing the node values.

## Output Format  

- Return array representing the zigzag level order traversal.
  

## Constraints  

- 1 ≤ n ≤ 1e4
- 1 ≤ node -> val ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search-tree