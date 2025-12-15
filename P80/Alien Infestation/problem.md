## Title
Alien Infestation

## Slug
alien-infestation

## Difficulty
Medium

## Description
Aliens spawn in the Cargo Bay (node 1) and rush the Bridge (node n).

The ship consists of $n$ decks connected by $m$ two-way lifts.
The aliens is attempting to travel from Cargo Bay (node 1) to the Bridge (node $n$).

To prevent this, you can disable specific lifts. Disabling a lift stops them.

Your task is to calculate the **minimum number of lifts** that must be disabled to completely sever all routes between Cargo Bay and the Bridge.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can disable edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of decks and lifts.
- The next $m$ lines describe the lifts. Each line contains two integers $a$ and $b$, indicating a lift between deck $a$ and deck $b$.

## Output Format
- Return one integer: the minimum number of lifts that need to be disabled.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
