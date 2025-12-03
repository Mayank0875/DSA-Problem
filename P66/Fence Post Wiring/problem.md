## Title
Fence Post Wiring

## Slug
fence-post-wiring

## Difficulty
Medium

## Description
Two parallel fences need electric wires connecting them to form a secure perimeter.

Two parallel fences, Inner Fence and Outer Fence, each contain n posts arranged in a line.
Inner Fence has an array `a` representing the ground height of each post.
Outer Fence has an array `b` representing the ground height of each post.

Inside each fence, adjacent posts are already connected by internal rails.

You must establish inter-fence wires connecting some posts of Inner Fence to some posts of Outer Fence.

The cost to create a wire between post i of Inner Fence and post j of Outer Fence is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single post is removed (from either Inner Fence or Outer Fence).
If one post fails and disappears along with all its connections, the remaining posts must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of posts:
1. post 1 from Inner Fence with post 2 from Outer Fence: cost |1-4| = 3.
2. post 3 from Inner Fence with post 2 from Outer Fence: cost |1-4| = 3.
3. post 2 from Inner Fence with post 1 from Outer Fence: cost |10-20| = 10.
4. post 2 from Inner Fence with post 3 from Outer Fence: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first post of Inner Fence with the first of Outer Fence, and the last post of Inner Fence with the last of Outer Fence, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of posts in each fence.
- The second line contains n integers representing the ground heights of Inner Fence.
- The third line contains n integers representing the ground heights of Outer Fence.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
