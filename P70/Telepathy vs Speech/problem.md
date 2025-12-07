## Title
Telepathy vs Speech

## Slug
telepathy-vs-speech

## Difficulty
Medium

## Description
Telepaths communicate via Mind Link. Others use Speech. Speech connects people who aren't Mind Linked.

The gathering has n guests numbered from 1 to n.
The Mind Net connects specific pairs of guests with direct links.
The Voice Net is constructed based on a unique rule:
A direct conversation exists between two guests if and only if there is no link connecting them.

Moving between any two connected guests takes exactly 1 hour on either network.
Two ideas, The Telepathic Thought and The Spoken Word, depart from guest 1 at the same time, heading for guest n.

1. The Telepathic Thought travels only using Mind Net.
2. The Spoken Word travels only using Voice Net.

To ensure safety, they must never arrive at the same guest at the same time (except for the final guest n).
Your task is to compute the minimum number of hours required for **both** ideas to reach guest n — specifically, the time when the slower idea arrives.
If either idea cannot reach guest n using their respective network, return -1.

## Examples

### 1

#### Input
4 2
1 3
3 4

#### Output
2

#### Explanation
The smallest possible time is 2. One takes the direct route (1 hour), the other takes a path of length 2.

### 2

#### Input
4 6
1 2
1 3
1 4
2 3
2 4
3 4

#### Output
-1

#### Explanation
The graph is fully connected for one network, meaning the complement network has no edges. The second idea cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of guests and the number of links.
- The next m lines each contain two integers u and v, representing a link between guests u and v.
- The graph is bidirectional. There is at most one link between any pair of guests.

## Output Format
- Return a single integer representing the minimum hours required for the last idea to arrive. If it is impossible, return -1.

## Constraints
- 2 ≤ n ≤ 400
- 0 ≤ m ≤ n(n - 1)/2
- 1 ≤ u, v ≤ n
- u ≠ v

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
